Category: Data_Visualization

Prompt style: Casual

Title: Budget Breakdown Tree Map

Prompt: Show me a budget breakdown as nested rectangles for three departments, each with a couple subcategories inside. Make each rectangle's size match its budget amount. Use darker colors for departments and lighter shades for their subcategories. Flag any subcategory taking up too much of its parent's budget by coloring it red. Below the tree map, show a summary with how each subcategory breaks down as a percentage of its department. When I hover over a rectangle, thicken the border and show the amount plus percentage of total. Load it with some realistic sample budget data.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three parent rectangles for departments                  | major  | The three parent rectangles establish the top-level budget structure for visual comparison.               | None         |
| 2   | state       | Size parent rectangles proportional to their dollar amounts      | major  | Proportional sizing allows users to compare department budgets visually at a glance.                      | None         |
| 3   | visual      | Display six subcategory rectangles nested inside parents         | major  | Nested subcategories show the detailed breakdown within each department budget.                           | C1           |
| 4   | layout      | Position subcategories fully inside their parent rectangles      | major  | Proper nesting visually communicates the hierarchical budget structure clearly.                           | C1, C3       |
| 5   | state       | Size subcategories proportional to their dollar amounts          | major  | Proportional subcategory sizing enables comparison of spending allocations within departments.            | C2           |
| 6   | layout      | Fit subcategories inside parent with no gaps between them        | major  | Gap-free space filling maximizes information density and creates a clean tree map appearance.             | C4, C5       |
| 7   | visual      | Use darker shade for parent rectangles                           | minor  | Darker shading helps parents stand out from children in the hierarchy.                                    | None         |
| 8   | visual      | Use lighter tint of same color family for subcategories          | minor  | Color tinting maintains visual connection between parents and their children through color relationships. | C7           |
| 9   | state       | Calculate which subcategories exceed 40% of parent budget        | major  | The 40% threshold calculation identifies budget concentration risks that need attention.                  | None         |
| 10  | visual      | Color subcategories red when exceeding 40% of parent             | major  | Red coloring draws immediate attention to budget risks for quick identification.                          | C9           |
| 11  | content     | Display summary bar below tree map                               | minor  | The summary bar provides detailed percentage breakdowns without cluttering the main visualization.        | None         |
| 12  | state       | Calculate each subcategory's percentage of its parent budget     | major  | Parent-relative percentages show how each department allocates its budget internally.                     | None         |
| 13  | content     | Show department name and subcategory percentages in summary      | major  | The summary gives users precise allocation data for the currently selected department.                    | C12          |
| 14  | interaction | Make border thicker when hovering over rectangle                 | minor  | Thicker borders provide clear visual feedback about which rectangle the user is examining.                | None         |
| 15  | content     | Display tooltip with exact dollar amount on hover                | major  | Exact amounts give users precise values that complement the visual proportions.                           | C14          |
| 16  | state       | Calculate percentage of total company budget for tooltip         | major  | Company-wide percentages help users understand each item's impact on the overall budget.                  | None         |

## Justification

The Budget Breakdown Tree Map achieved 50% pass rate (8/16 criteria) with failures concentrated in layout precision and calculation logic. The visualization correctly displays three parent rectangles for Engineering, Marketing, and Operations (C1 passed) with six nested subcategory rectangles (C3 passed). The parent rectangle sizing is proportional to dollar amounts - Engineering occupies roughly half the space, Marketing a third, and Operations the remainder (C2 passed). However, the model failed C4 by allowing subcategory rectangles to overflow outside their parent boundaries, with Tools extending beyond Engineering's border. The space-filling algorithm failed C6, leaving visible white gaps between Salaries and Tools inside Engineering instead of filling the parent rectangle completely. Subcategory sizing was inconsistent (C5 failed) - Ads ($25K) and Events ($15K) appeared nearly equal in size despite the significant value difference. The color scheme worked partially: parents used darker shades (C7 passed) but subcategories failed C8 by using completely different colors instead of lighter tints of their parent's color family. The budget risk calculation failed C9 and C10 - Salaries ($45K = 75% of Engineering's $60K) should be red for exceeding 40% of parent, but appeared in the default color instead. The summary bar displayed below (C11 passed) but failed C12 and C13 by showing percentages of total company budget instead of calculating each subcategory's percentage relative to its parent department. Hover interactions worked correctly, thickening borders (C14 passed) and showing tooltips with dollar amounts (C15 passed), and the percentage of total company budget calculated correctly in the tooltip (C16 passed).
