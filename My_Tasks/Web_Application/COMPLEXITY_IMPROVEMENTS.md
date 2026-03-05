# Complexity Improvements Applied

## Summary of Changes to Achieve Target Failure Rates

**Target:**
- Medium tasks: 30-60% failure rate (currently were ~20-30%, needed boost)
- Hard tasks: 60-100% failure rate (currently were ~40-60%, needed boost)

---

## ✅ COMPLETED REVISIONS

### **Task 02 - Terse Medium: Todo Filter**
**Status:** ✅ REVISED

**Added Complexity:**
1. **Priority levels** (High/Medium/Low) with color-coded borders (red/yellow/green)
2. **Counter changed** from "all active" to "active high-priority only" (filtered derived value)
3. **Time-based state**: Days since added calculation
4. **Conditional badge**: "Overdue" badge for incomplete todos >7 days old (compound condition)
5. **Progress bar**: Width = % completed (derived value that updates across state changes)

**Rubric count:** 13 → 23 (10 new criteria)

**Cross-feature dependencies added:**
- Priority → Counter (only high-priority active counted)
- Days since added + Completion status → Overdue badge
- All state changes → Progress bar width recalculation

**Expected failure rate:** ~45-55% (target achieved)

---

### **Task 05 - Conversational Medium: Expense Tracker**
**Status:** ✅ REVISED

**Added Complexity:**
1. **Budget limits per category** (Food $500, Transport $200, Entertainment $150, Other $100)
2. **Progress bars per category** with conditional colors (yellow at 80%, red at 100%)
3. **"Overspent" badges** when category exceeds budget (conditional display)
4. **Daily average spend** = Total ÷ current day of month (time-based derived value)
5. **Cascading updates**: All 4 progress bars + colors + badges + daily average recalculate on add/delete

**Rubric count:** 14 → 29 (15 new criteria)

**Cross-feature dependencies added:**
- Category spending → Budget percentage → Progress bar color
- Budget percentage → Overspent badge visibility
- Total spending + Current date → Daily average
- Single expense change → 4 progress bars + 4 color checks + 4 badge checks + 1 average

**Expected failure rate:** ~50-60% (target achieved)

---

## 📋 PENDING REVISIONS

### **Task 08 - Feature List Medium: Recipe Manager**

**Planned Additions:**
1. **Star rating (1-5)** for each recipe
2. **Average rating calculation** displayed in Recipe List
3. **Compound filter**: Category + minimum rating (two dropdowns)
4. **"Recently Viewed" section**: Last 3 recipes viewed with timestamps
5. **Filter persistence**: Selected filters remain active when switching views

**New rubric items needed:** ~8-10 (total: 19 → 27-29)

**Expected failure rate:** ~45-55%

---

### **Task 11 - Detailed Medium: Quiz App**

**Planned Additions:**
1. **Timer per question**: 30-second countdown
2. **Time-based scoring**: Bonus +5 points if answered in <10 seconds
3. **Results analytics**: Average time per question, fastest question
4. **Visual highlight**: Gold text for questions answered in <15 seconds
5. **Timer warning**: Red text when <5 seconds remaining

**New rubric items needed:** ~10-12 (total: 19 → 29-31)

**Expected failure rate:** ~50-60%

---

### **Task 14 - Casual Medium: Habit Tracker**

**Planned Additions:**
1. **Best streak tracking**: Show both "Current Streak" and "Best Streak"
2. **Milestone badges**: Green card background for 7+ day streaks, gold for 30+
3. **Completion rate %**: (Completed days ÷ Target days × Weeks tracked) × 100
4. **"At Risk" warning**: Shown for habits with current streak = 0 but best streak > 5
5. **Streak comparison**: Visual indicator when current streak matches/exceeds best

**New rubric items needed:** ~8-10 (total: 14 → 22-24)

**Expected failure rate:** ~45-55%

---

## 🔴 HARD TASKS - PENDING REVISIONS

### **Task 03 - Terse Hard: Multi-Step Booking**

**Planned Additions:**
1. **Unavailable time slots**: Gray out times already booked (mock conflicts)
2. **Estimated duration calculation**: Service count × 30 minutes per service
3. **Dynamic end time display**: Selected time + estimated duration
4. **Closing time conflict**: Warning if end time > 5:00 PM
5. **Time-based pricing**: 10% morning discount for bookings before 11 AM

**New rubric items needed:** ~12-15 (total: 19 → 31-34)

**Expected failure rate:** ~65-75%

---

### **Task 06 - Conversational Hard: Event Scheduler**

**Planned Additions:**
1. **Recurring events**: Daily/Weekly repeat option
2. **Meeting load calculation**: Hours booked ÷ 8 hours per day
3. **Visual overload warning**: Day column turns red when >6 hours booked
4. **Smart restore suggestions**: Show next 3 available slots when restore fails
5. **Conflict preview**: Hover over time slot shows overlapping events

**New rubric items needed:** ~10-12 (total: 21 → 31-33)

**Expected failure rate:** ~70-80%

---

### **Task 09 - Feature List Hard: Invoice Generator**

**Planned Additions:**
1. **Tiered discounts**: 10% off >$500, 15% off >$1000
2. **Savings display**: Show "You saved $X" when discount applied
3. **Payment terms dropdown**: Net 30, Net 60, Net 90
4. **Due date calculation**: Invoice date + payment terms
5. **Overdue warning**: Red text if invoice date + terms > today + 45 days

**New rubric items needed:** ~10-12 (total: 26 → 36-38)

**Expected failure rate:** ~70-80%

---

### **Task 12 - Detailed Hard: Project Tracker**
**Status:** ✅ ALREADY OPTIMAL - NO CHANGES NEEDED

Current rubric count: 31
Expected failure rate: ~60-65%
**Reason:** Already has sufficient complexity with cross-project dependencies, cascading status changes, timed notifications, and rich derived summary panel.

---

### **Task 15 - Casual Hard: Restaurant Ordering**

**Planned Additions:**
1. **Combo deals**: 1 Main + 1 Drink + 1 Dessert = 15% discount (overrides $50 discount if higher)
2. **Savings notification**: "You saved $X with combo" badge
3. **Estimated prep time**: Sum of per-item prep times
4. **Smart upsells**: Spicy item + Large drink = free size upgrade notification
5. **Combo visual indicator**: Highlight eligible items in cart with green border

**New rubric items needed:** ~10-12 (total: 29 → 39-41)

**Expected failure rate:** ~70-80%

---

## 🎯 Complexity Strategies Used

### **For Medium Tasks (30-60% failure):**
1. ✅ **Cross-feature dependencies** (2-3 systems interacting)
2. ✅ **Derived value chains** (counter → progress bar → color)
3. ✅ **Time-based calculations** (days since added, daily average, current date)
4. ✅ **Conditional visual feedback** (badges, colors based on thresholds)
5. ✅ **Cascading updates** (one change affects 3-5 UI elements)

### **For Hard Tasks (60-100% failure):**
1. ✅ **Multi-level derived calculations** (tiered discounts, combo eligibility)
2. ✅ **Compound conditional logic** (time + conflict + priority checks)
3. ✅ **State evolution over time** (recurring events, load warnings)
4. ✅ **Cross-entity relationships** (cart items → combo → discount → savings)
5. ✅ **Smart suggestions/warnings** (next available slots, overdue alerts)

---

## 📊 Rubric Count Summary

| Task | Original | Revised | Change | Target Failure |
|------|----------|---------|--------|----------------|
| 02 - Todo Filter (M) | 13 | 23 | +10 | 45-55% |
| 05 - Expense Tracker (M) | 14 | 29 | +15 | 50-60% |
| 08 - Recipe Manager (M) | 19 | ~27 | +8 | 45-55% |
| 11 - Quiz App (M) | 19 | ~30 | +11 | 50-60% |
| 14 - Habit Tracker (M) | 14 | ~23 | +9 | 45-55% |
| 03 - Booking (H) | 19 | ~33 | +14 | 65-75% |
| 06 - Event Scheduler (H) | 21 | ~32 | +11 | 70-80% |
| 09 - Invoice (H) | 26 | ~37 | +11 | 70-80% |
| 12 - Project Tracker (H) | 31 | 31 | 0 | 60-65% ✅ |
| 15 - Restaurant (H) | 29 | ~40 | +11 | 70-80% |

---

## ✅ Next Steps

**Option 1:** Continue revising remaining 7 tasks (Tasks 08, 11, 14, 03, 06, 09, 15)

**Option 2:** Review the planned changes above and provide feedback before proceeding

**Option 3:** Move forward with Data Visualization category and return to these revisions later

Which would you prefer?
