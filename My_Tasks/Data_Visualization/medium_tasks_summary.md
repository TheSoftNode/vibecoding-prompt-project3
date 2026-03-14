# Data Visualization Medium Tasks Summary

## Overview
10 unique Medium difficulty Data Visualization tasks created following the pattern analysis from `medium_task_examples.md`.

**Target:** 40-60% pass rate (Medium difficulty)
**Features per task:** 3-5 interconnected features
**Criteria per task:** 16-20 max

---

## Tasks Created

### **Casual Style (3 tasks)**

#### 1. Energy Flow Sankey Diagram
**File:** `Casual/16_casual_medium_energy_flow.md`
**Visualization:** Sankey diagram
**Patterns:** Multi-View Coordination + Proportional Sizing + Filtering with Subset Recalc + Edge Cases
**Features:** 5
**Criteria:** 16
**Target Pass Rate:** 56% (9/16)

**Key Failure Points:**
- Curved paths (models draw straight lines) ~55% fail
- Proportional thickness calculations ~50% fail
- Edge case grouping <3% flows ~60% fail
- Efficiency calculation from flow percentage ~45% fail
- Summary recalculates from clicked source only ~50% fail

---

#### 2. Budget Breakdown Tree Map
**File:** `Casual/17_casual_medium_budget_treemap.md`
**Visualization:** Tree map with nested rectangles
**Patterns:** Conditional Visual States + Derived Calculations + Proportional Sizing + Zone-Based Logic
**Features:** 4
**Criteria:** 16
**Target Pass Rate:** 50% (8/16)

**Key Failure Points:**
- Proportional rectangle sizing ~45% fail
- Perfect nesting without gaps ~55% fail
- Parent fills exactly with children ~60% fail
- Red coloring when >40% of parent ~50% fail
- Calculate % of parent for each child ~45% fail
- Color tinting (lighter shade of same family) ~40% fail

---

#### 3. Team Collaboration Network Graph
**File:** `Casual/18_casual_medium_team_network.md`
**Visualization:** Network graph
**Patterns:** Multi-View Coordination + Conditional Visual States + Absolute Position-Based Rules + Live Updates
**Features:** 5
**Criteria:** 16
**Target Pass Rate:** 56% (9/16)

**Key Failure Points:**
- Circle sizing by connection count ~40% fail
- No overlapping circles ~55% fail
- Connected members positioned closer ~60% fail
- Lines don't cross through circles ~65% fail
- Network density calculation (actual/28) ~50% fail
- Deselect on second click ~45% fail
- Gray out non-connected on selection ~40% fail

---

### **Conversational Style (3 tasks)**

#### 4. Quarterly Sales Performance Multi-Ring Chart
**File:** `Conversational/06_conversational_medium_sales_ring.md`
**Visualization:** Multi-ring radial chart
**Patterns:** Conditional Visual States + Derived Calculations + Zone-Based Logic + Edge Cases
**Features:** 4
**Criteria:** 16
**Target Pass Rate:** 56% (9/16)

**Key Failure Points:**
- Arc angles proportional to % of quarter total ~50% fail
- Segment alignment across rings (same start angle) ~60% fail
- Green/red/gray coloring based on previous quarter ~45% fail
- Q1 gray (no prior quarter) ~50% fail
- Growth rate Q1→Q3 only ~40% fail
- Most consistent = smallest variance ~55% fail
- Tie-breaker: higher Q3 sales ~65% fail

---

#### 5. Customer Journey Chord Diagram
**File:** `Conversational/07_conversational_medium_journey_chord.md`
**Visualization:** Chord diagram
**Patterns:** Proportional Sizing + Multi-View Coordination + Filtering with Subset Recalc + Edge Cases
**Features:** 5
**Criteria:** 16
**Target Pass Rate:** 50% (8/16)

**Key Failure Points:**
- Ribbon width proportional to flow volume ~50% fail
- Directional flows (Website→Email ≠ Email→Website) ~55% fail
- Inbound sum (flows INTO touchpoint) vs outbound ~45% fail
- Net flow = inbound - outbound ~40% fail
- Green/red coloring of net value ~35% fail
- Group flows <50 into dashed "Low Traffic" ribbon ~65% fail
- Ribbons don't overlap touchpoint arcs ~60% fail

---

#### 6. Regional Sales Heatmap Grid
**File:** `Conversational/08_conversational_medium_regional_heatmap.md`
**Visualization:** Heatmap grid
**Patterns:** Conditional Visual States + Derived Calculations + Filtering with Subset Recalc + Sliding Window
**Features:** 4
**Criteria:** 16
**Target Pass Rate:** 50% (8/16)

**Key Failure Points:**
- Color based on region's own average (not global) ~55% fail
- Recalculate average when filter changes ~60% fail
- Yellow for within 5% of average ~50% fail
- Darker shades for farther from average ~45% fail
- Highest = most months above its average ~50% fail
- Tie-breaker: first in row order ~65% fail
- Grid redraws with only filtered months as columns ~40% fail

---

### **Feature_List Style (4 tasks)**

#### 7. Revenue Waterfall Chart
**File:** `Feature_List/09_featurelist_medium_revenue_waterfall.md`
**Visualization:** Waterfall chart
**Patterns:** Derived Calculations + Conditional Visual States + Proportional Sizing + Edge Cases
**Features:** 5
**Criteria:** 16
**Target Pass Rate:** 56% (9/16)

**Key Failure Points:**
- Bars float at correct heights (not all starting at zero) ~60% fail
- Connector lines between bars ~50% fail
- Net change = ending - opening ~40% fail
- Green/red formatting of net change label ~45% fail
- Largest increase/decrease identification ~40% fail
- Bar heights proportional to amounts ~35% fail

---

#### 8. Inventory Distribution Bubble Chart
**File:** `Feature_List/10_featurelist_medium_inventory_bubble.md`
**Visualization:** Bubble chart
**Patterns:** Proportional Sizing + Multi-View Coordination + Conditional Visual States + Derived Calculations
**Features:** 4
**Criteria:** 16
**Target Pass Rate:** 56% (9/16)

**Key Failure Points:**
- Bubble area proportional to value ~50% fail (use diameter instead of area)
- Stock-to-velocity ratio calculation (stock/velocity) ~45% fail
- Risk thresholds (<2, 2-4, >4 months) ~55% fail
- No bubble overlaps ~60% fail
- Ratio displayed in months with one decimal ~40% fail
- Proportional positioning on both axes ~35% fail

---

#### 9. Employee Performance Parallel Coordinates
**File:** `Feature_List/11_featurelist_medium_performance_parallel.md`
**Visualization:** Parallel coordinates
**Patterns:** Multi-View Coordination + Filtering with Subset Recalc + Conditional Visual States + Zone-Based Logic
**Features:** 5
**Criteria:** 16
**Target Pass Rate:** 50% (8/16)

**Key Failure Points:**
- Star rating conversion (5 stars = 100 on scale) ~50% fail
- Line thickness based on Quality zones ~55% fail
- Filter requires matching BOTH ranges ~60% fail (use OR instead of AND)
- Averages calculated from visible only ~50% fail
- "No employees match" when count = 0 ~45% fail
- Count updates dynamically with filters ~40% fail
- Three thickness levels (thick/medium/thin) for three zones ~55% fail

---

#### 10. Market Share Evolution Stacked Area Chart
**File:** `Feature_List/12_featurelist_medium_market_stacked.md`
**Visualization:** Stacked area chart
**Patterns:** Derived Calculations + Conditional Visual States + Proportional Sizing + Filtering with Subset Recalc
**Features:** 4
**Criteria:** 20 (exception - more complex)
**Target Pass Rate:** 50% (10/20)

**Key Failure Points:**
- Areas stack to 100% at each quarter ~45% fail
- Smooth curves between points ~55% fail
- Trend calculated from selected period only ~60% fail
- Trend thresholds (>2 points growth/shrink) ~50% fail
- "Stable" for changes within ±2 points ~45% fail
- Badges update when filter changes ~55% fail
- Vertical stacking order (A, B, C, D bottom-to-top) ~40% fail

---

## Pattern Coverage Across All 10 Tasks

| Pattern | Tasks Using It | Count |
|---------|----------------|-------|
| Multi-View Coordination | #1, #3, #5, #8, #9 | 5 |
| Conditional Visual States | #2, #4, #6, #7, #8, #9, #10 | 7 |
| Derived Calculations | #2, #4, #6, #7, #8, #10 | 6 |
| Proportional Sizing | #1, #2, #5, #7, #8, #10 | 6 |
| Filtering with Subset Recalc | #1, #5, #6, #9, #10 | 5 |
| Edge Cases | #1, #4, #5, #7 | 4 |
| Zone-Based Logic | #2, #4, #9 | 3 |
| Absolute Position-Based Rules | #3 | 1 |
| Live Updates | #3 | 1 |
| Sliding Window | #6 | 1 |

**Most common patterns:**
1. Conditional Visual States (7 tasks)
2. Derived Calculations (6 tasks)
3. Proportional Sizing (6 tasks)

---

## Visualization Types - All Unique

1. Sankey diagram (Energy Flow)
2. Tree map (Budget Breakdown)
3. Network graph (Team Collaboration)
4. Multi-ring radial chart (Sales Performance)
5. Chord diagram (Customer Journey)
6. Heatmap grid (Regional Sales)
7. Waterfall chart (Revenue)
8. Bubble chart (Inventory Distribution)
9. Parallel coordinates (Employee Performance)
10. Stacked area chart (Market Share)

**No overlaps with existing medium_task_examples.md:**
- No simple bar charts
- No pie charts
- No basic scatter plots
- No line charts with standard axes

---

## Key Differentiators from Examples

### 1. Visual/Geometric Complexity
- Examples rely on calculation complexity
- Our tasks add arc calculations, curved paths, nested rectangles, node positioning

### 2. Spatial Relationships
- Examples test logic
- We test visual proportions (path width proportional to value, arc angles, rectangle sizing)

### 3. Natural Failure Surfaces
- **Curved vs straight:** Sankey, Chord (~55-65% draw straight)
- **Area vs diameter:** Bubble chart (~50% use diameter instead of area)
- **Floating vs grounded:** Waterfall (~60% start all bars at zero)
- **Stacking to 100%:** Stacked area (~45% have gaps or overlaps)
- **Directional flows:** Chord diagram (~55% treat as bidirectional)

### 4. Testable Without Pixel Values
- "Band thickness represents percentage" (visual comparison)
- "30-min bar exactly twice as tall as 15-min bar" (proportional ratio)
- "Areas sum to 100% at each quarter" (constraint verification)
- "Ribbons don't overlap touchpoint arcs" (visual inspection)

---

## Success Criteria Met

✅ All 10 tasks use different visualization types
✅ All different from medium_task_examples.md
✅ All have 3-5 features
✅ All combine 3-4 failure patterns
✅ Target pass rate: 50-56% (within 40-60% Medium range)
✅ Distributed across 3 styles: Casual (3), Conversational (3), Feature_List (4)
✅ All prompts testable without giving away pixel values
✅ All justifications written in human tone with specific failure examples
