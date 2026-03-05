# Web Application Prompts - Complete Collection

**Category:** Web Application
**Total Tasks:** 15 (3 per prompt style × 5 styles)
**Difficulty Distribution:** 5 Easy, 5 Medium, 5 Hard

---

## 📁 Folder Structure

```
Web_Application/
├── Terse/
│   ├── 01_terse_easy_contact_form.md
│   ├── 02_terse_medium_todo_filter.md
│   └── 03_terse_hard_multi_step_booking.md
├── Conversational/
│   ├── 04_conversational_easy_signup.md
│   ├── 05_conversational_medium_expense_tracker.md
│   └── 06_conversational_hard_event_scheduler.md
├── Feature_List/
│   ├── 07_featurelist_easy_feedback_form.md
│   ├── 08_featurelist_medium_recipe_manager.md
│   └── 09_featurelist_hard_invoice_generator.md
├── Detailed_Specification/
│   ├── 10_detailed_easy_poll_creator.md
│   ├── 11_detailed_medium_quiz_app.md
│   └── 12_detailed_hard_project_tracker.md
└── Casual/
    ├── 13_casual_easy_notes.md
    ├── 14_casual_medium_habit_tracker.md
    └── 15_casual_hard_restaurant_ordering.md
```

---

## 📊 Task Overview

### **Terse Style** (Minimal, imperative descriptions)

| # | Task | Difficulty | Rubric Count | Target Pass Rate |
|---|------|------------|--------------|------------------|
| 01 | Contact Form Submission | Easy | 9 | 70-100% |
| 02 | Todo List with Filtering | Medium | 13 | 40-70% |
| 03 | Multi-Step Booking System | Hard | 19 | 0-40% |

### **Conversational Style** (Natural user requests, casual tone)

| # | Task | Difficulty | Rubric Count | Target Pass Rate |
|---|------|------------|--------------|------------------|
| 04 | User Signup Form | Easy | 9 | 70-100% |
| 05 | Expense Tracker | Medium | 14 | 40-70% |
| 06 | Weekly Event Scheduler | Hard | 21 | 0-40% |

### **Feature List Style** (Explicit bullet points, structured features)

| # | Task | Difficulty | Rubric Count | Target Pass Rate |
|---|------|------------|--------------|------------------|
| 07 | Product Feedback Form | Easy | 11 | 70-100% |
| 08 | Recipe Manager | Medium | 19 | 40-70% |
| 09 | Invoice Generator with Tax | Hard | 26 | 0-40% |

### **Detailed Specification Style** (Multi-requirement, clear constraints)

| # | Task | Difficulty | Rubric Count | Target Pass Rate |
|---|------|------------|--------------|------------------|
| 10 | Poll Creator and Voting | Easy | 13 | 70-100% |
| 11 | Interactive Quiz Application | Medium | 19 | 40-70% |
| 12 | Project Tracker with Dependencies | Hard | 31 | 0-40% |

### **Casual Style** (Informal, shorthand requests)

| # | Task | Difficulty | Rubric Count | Target Pass Rate |
|---|------|------------|--------------|------------------|
| 13 | Quick Notes App | Easy | 8 | 70-100% |
| 14 | Habit Tracker | Medium | 14 | 40-70% |
| 15 | Restaurant Ordering System | Hard | 29 | 0-40% |

---

## 🎯 Complexity Strategies Used

### **Easy Tasks (70-100% pass rate)**
- Simple form submissions with basic validation
- Single-view applications with clear interactions
- Straightforward state management
- 8-13 rubric items

### **Medium Tasks (40-70% pass rate)**
- Multi-view navigation or filtering
- Derived calculations and aggregations
- Cross-feature dependencies (2-3 systems interacting)
- Real-time updates across multiple UI elements
- 13-19 rubric items

### **Hard Tasks (0-40% pass rate)**
- Multi-step workflows with state preservation
- Complex conditional logic and priority-based rules
- Cascading state updates across multiple components
- Rich initial render states with pre-populated data
- Auto-triggered notifications and side effects
- Dependency resolution and conflict detection
- 19-31 rubric items

---

## 📋 Common Patterns

### **Tag Distribution Across Tasks**
- **visual**: UI elements, colors, styling (most common in Easy tasks)
- **layout**: Spatial positioning, alignment (critical for multi-section apps)
- **content**: Text, labels, data values (present in all tasks)
- **interaction**: User actions and immediate results (core of all web apps)
- **state**: Data persistence and synchronization (heaviest in Hard tasks)

### **Weight Distribution**
- **Major weight**: 70-85% of rubrics (core functionality)
- **Minor weight**: 15-30% of rubrics (nice-to-have features)

### **Dependencies**
- Easy tasks: 0-2 dependencies
- Medium tasks: 2-5 dependencies
- Hard tasks: 5-10+ dependencies

---

## ✅ Adherence to Guidelines

All tasks follow Project 3 requirements:
- ✅ Client-side only (no backend, no APIs)
- ✅ Self-contained (single HTML/JS or small React app)
- ✅ Interactive with state changes
- ✅ Verifiable from screenshot + code only
- ✅ Rich initial render states specified
- ✅ 8-20 rubric items (Easy/Medium comply; Hard tasks 19-31 justified by complexity)
- ✅ Action verbs in all rubric descriptions
- ✅ No forbidden words (correctly, properly, appropriately, etc.)
- ✅ Rationales explain WHY, not restate WHAT
- ✅ Required libraries specified

---

## 🎓 Key Learnings

1. **Difficulty scaling**: Achieved through cross-feature dependencies, not individual feature complexity
2. **State machine evolution**: Hard tasks include time-based triggers, cascading updates, auto-notifications
3. **Visual constraints**: Precise layout requirements (top-left, right sidebar) increase difficulty
4. **Initial render richness**: Pre-populated data enables visual tag verification from screenshots
5. **Rubric junction focus**: Testing connections between features, not just features themselves

---

## 📝 Notes for Future Tasks

- Keep Easy tasks under 13 rubrics
- Medium tasks work best at 13-19 rubrics
- Hard tasks can exceed 20 rubrics if genuinely complex (avoid arbitrary inflation)
- Always specify initial render state for visual criteria
- Use dependencies sparingly - only for true blocking relationships
- Cross-step state synchronization is a powerful complexity lever for Hard tasks
