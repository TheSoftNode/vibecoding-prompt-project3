# Medium Task Pattern Analysis
## Deep Analysis of What Makes Medium Tasks Achieve 40-60% Failure Rate

This document analyzes the patterns from `medium_task_examples.md` to understand what makes them effectively challenging for AI models.

---

## 10 Core Patterns That Drive Model Failures

### **Pattern 1: Multi-View Coordination with Cross-Updates**

**Examples:** Freelancer dashboard (#1), Drone assembly heatmap (#3)

**The Pattern:**
- Multiple visualizations (bar chart + pie chart + metrics card)
- **Click in one view → updates ALL other views**
- Each view shows different slice of same data
- Synchronized state across views

**Why Models Fail:**
- Managing shared state across 3+ components (~40% fail)
- Event propagation from one chart to update others (~50% fail)
- Recalculating derived metrics from filtered subset (~45% fail)

**Key Phrase to Use:** "Click bar to update pie and metrics"

---

### **Pattern 2: Complex Multi-Factor Calculations with Derived Displays**

**Examples:** Risk heatmap (#2), Sprint Velocity Dashboard (#5)

**The Pattern:**
- **Multiple inputs feed into complex formula**
- Display derived values in multiple places
- Conditional logic based on calculations (flags, colors, badges)
- **Recalculates on ANY input change**

**Example from Risk Heatmap:**
- Risk = f(effort/person, dependencies/people ratio, time pressure)
- Heatmap color = task's % of total portfolio risk
- Flag tasks > equal split
- Top 3 panel shows % breakdown

**Why Models Fail:**
- Multi-factor formulas (~55% get formula wrong)
- Proportional calculations (task's share of TOTAL) (~50% fail)
- Conditional flagging based on threshold (~40% fail)
- Multiple derived displays staying in sync (~45% fail)

**Key Phrases to Use:** "Recalculates upon input change", "share of portfolio risk", "flagged"

---

### **Pattern 3: Conditional Visual States Based on Computed Comparisons**

**Examples:** Sprint Velocity bars colored by rolling average comparison (#5)

**The Pattern:**
- Compute rolling/moving average (state calculation)
- **Compare each data point to computed value**
- Apply different visual treatment based on comparison
- Handle edge cases (first N items have different logic)

**Specific Example:**
```
- Rolling average starting at sprint 3
- Bar green if >= rolling average at that position
- Bar red if < rolling average
- Sprints 1-2 are blue (no average yet)
```

**Why Models Fail:**
- Computing rolling average correctly (~35% fail)
- **Positional comparison** (bar 5 compared to rolling avg AT position 5) (~55% fail)
- Edge case handling (first 2 sprints different logic) (~50% fail)
- Three-way conditional coloring (~40% fail)

---

### **Pattern 4: Dynamic Filtering with Subset Recalculation**

**Examples:** Sprint Velocity (#5), Trekking profiles (#8)

**The Pattern:**
- Filter buttons affect what's visible
- **Summary stats recalculate from FILTERED subset only** (not all data)
- Multiple summary fields with different logic
- Tie-breaking rules for edge cases

**Specific Example from Sprint Velocity:**
```
- Filter: All / Above Target / Below Target
- Summary recalculates from FILTERED data only:
  - Average (from visible sprints)
  - Best/worst (from visible, latest if tie)
  - Count above target (from visible)
  - Trend badge (last vs second-to-last WITH rolling avg)
```

**Why Models Fail:**
- Recalculating from filtered subset (~50% fail to filter correctly)
- Tie-breaking "latest in sequence" (~60% ignore this)
- Conditional badge logic with % thresholds (~55% fail)
- "N/A" when insufficient data (~45% forget edge case)

---

### **Pattern 5: Proportional/Relative Visual Sizing**

**Examples:** Workout bars (#7), Therapy jar (#6)

**The Pattern:**
- Visual element size **proportional to value**
- Explicit ratio stated: "30-minute bar exactly twice as tall as 15-minute"
- Or: "Jar fills proportionally to total/300 minutes"

**Why Models Fail:**
- Fixed heights instead of proportional (~40% fail)
- Wrong ratio calculation (~35% fail)

**Key Phrase to Use:** "exactly twice as tall", "proportionally to"

---

### **Pattern 6: Sliding Window Display with Persistent State**

**Examples:** Workout visualizer (#7)

**The Pattern:**
- **Display max N items** (sliding window)
- **Store ALL items** (persistent state)
- Visual property based on ABSOLUTE position (1st, 2nd, 3rd...) not visual slot
- Running totals include removed items

**Specific Example:**
```
- Chart shows max 5 bars (remove oldest when 6th added)
- Color alternates by TOTAL count (6th workout is green even in 5th slot)
- Total Time accumulates ALL workouts (even removed from display)
```

**Why Models Fail:**
- Coloring by absolute index vs visual index (~60% fail)
- Running total including invisible items (~50% fail)
- Sliding window logic (~40% fail)

---

### **Pattern 7: Zone-Based Conditional Logic with Asymmetric Patterns**

**Examples:** Trekking altitude zones (#8)

**The Pattern:**
- Data categorized into zones with different rules per zone
- **Asymmetric patterns** (ascent ≠ descent)
- Speed ranges vary by zone
- Time % allocation across zones

**Specific Example:**
```
- 3 zones with altitude ranges (0-2000m, 2001-3000m, >3000m)
- Different speed ranges per zone
- 40% / 15% / 45% time split across zones
- Ascent skips Treeline zone, descent includes all zones
```

**Why Models Fail:**
- Asymmetric ascent/descent (~65% make them symmetric)
- Zone-specific constraints (~50% apply wrong ranges)
- Time allocation % (~45% fail to match)

---

### **Pattern 8: Live Bidirectional Sync**

**Examples:** Markdown-to-Mindmap (#4)

**The Pattern:**
- Input panel + visual output panel
- **Changes in input instantly update output** (no button needed)
- Initial state pre-filled (visible on load)
- Complex layout algorithm (no overlaps, neat spacing)

**Why Models Fail:**
- Live updates without explicit trigger (~40% need button)
- Layout algorithm preventing overlaps (~55% have overlaps)
- Initial render with sample data (~30% blank on load)

**Key Phrase to Use:** "updates live while typing", "pre-fill with example", "no overlaps"

---

### **Pattern 9: Absolute Position-Based Rules Across Operations**

**Examples:** Workout color alternation (#7), Image features (#9)

**The Pattern:**
- Visual property determined by absolute sequence number
- Persists across deletions/additions
- Not affected by what's currently visible

**Example:** 6th workout is green even when displayed in 5th slot

**Why Models Fail:**
- Tracking absolute vs relative position (~60% fail)

---

### **Pattern 10: Step-by-Step Animation with Synchronized Counters**

**Examples:** MinHeap visualizer (#10)

**The Pattern:**
- Algorithm steps shown one-by-one (not instant)
- Counter tracking operations (swap count)
- **Counter updates WITH each animation step** (synchronized)
- Multiple synchronized displays (tree, sorted list, counter)

**Why Models Fail:**
- Step-by-step animation (~50% show final state only)
- Synchronized counter updates (~55% update only at end)
- Correct algorithm visualization (~45% wrong steps)

---

## Common Failure-Inducing Elements Across All Examples

### **A. Mathematical/Computational Complexity**
1. **Rolling/moving averages** (not simple average)
2. **Proportional calculations** (share of total, percentages)
3. **Multi-factor formulas** (weighted combinations)
4. **Positional comparisons** (compare item N to computed value at position N)

### **B. State Management Complexity**
1. **Filtered subset recalculation** (stats from visible only, not all data)
2. **Absolute vs relative indexing** (6th item vs 5th slot)
3. **Persistent state with sliding window** (display 5, store all)
4. **Synchronized multi-component state** (update 3 charts from 1 click)

### **C. Conditional Logic Complexity**
1. **Multi-way conditionals** (green/red/blue based on different rules)
2. **Edge case handling** (first 2 items different logic, "N/A" when insufficient data)
3. **Tie-breaking rules** ("latest in sequence" when tied)
4. **Zone-based rules** (different behavior per category)

### **D. Visual/Layout Complexity**
1. **Proportional sizing** (explicit ratios like "2x as tall")
2. **Precise spatial relationships** ("to the right", "aligned", "no overlaps")
3. **Conditional visual states** (color changes based on computation)
4. **Custom shapes/layouts** (hexagon, trapezoid, diamond panels)

### **E. Interaction Complexity**
1. **Cross-view updates** (click bar → update pie + metrics)
2. **Live updates without button** (type → instant render)
3. **Filtering affecting multiple displays** (filter → chart + summary both update)
4. **Step-by-step animations** (not instant state change)

---

## Recommended Formula for Data Visualization Medium Tasks

A strong Medium Data Viz task should combine **3-4 of these patterns**:

### **Best Pattern Combination:**

1. **Multi-View Coordination** (Pattern 1)
   - 2-3 different chart types showing related data
   - Click/select in one updates others

2. **Complex Derived Calculations** (Pattern 2)
   - Multi-factor formula or proportional calculations
   - Display results in multiple places

3. **Conditional Visual States** (Pattern 3)
   - Color/size/style changes based on computed comparisons
   - Edge case handling (different rules for subset)

4. **Filtering with Subset Recalculation** (Pattern 4)
   - Filter buttons
   - Summary stats recalculate from filtered data only
   - Tie-breaking or N/A logic

### **For Data Visualization Category Specifically:**

**Recommended approach:**
- Sankey/flow diagram OR multi-ring chart OR network graph (natural visual complexity)
- + Click segment to filter connected view
- + Summary panel showing proportions from clicked/filtered subset
- + Conditional highlighting when values exceed threshold
- + Edge case: values below X% grouped as "Other"

**This hits:**
- Multi-view coordination ✓
- Proportional calculations ✓
- Conditional visuals ✓
- Filtering with recalculation ✓
- Edge cases ✓

---

## Key Insights for Prompt Writing

### **What to Include:**
1. **Explicit ratios/proportions** - "twice as tall", "share of total"
2. **Edge case rules** - "first 2 use blue", "if tied, pick latest"
3. **Recalculation triggers** - "recalculates upon input change", "updates from filtered data only"
4. **Cross-component updates** - "clicking updates all three views"
5. **Positional comparisons** - "compare each bar to rolling average at that position"

### **What to Avoid:**
1. Giving exact pixel values (not testable without giving away answer)
2. Single isolated features (need interaction between 3-5 features)
3. Simple averages (use rolling/moving/weighted instead)
4. Static displays (need dynamic updates/recalculations)

### **Testability Without Giving Answers:**
- Use relative descriptions: "twice as tall", "aligned with", "proportional to"
- Use visual relationships: "bars sized to match their values"
- Use comparative language: "larger categories get more space"
- Avoid absolute measurements: not "200px wide" but "width matches legend width"
