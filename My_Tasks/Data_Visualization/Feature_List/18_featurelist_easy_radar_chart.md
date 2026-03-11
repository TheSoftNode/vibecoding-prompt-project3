Category: Data_Visualization

Prompt style: Feature_List

Title: Skill Radar Chart

Prompt: Build a radar chart showing skill proficiency with these features:
- Display a pentagon-shaped radar chart with 5 axes labeled "Coding", "Design", "Communication", "Leadership", "Problem Solving", each extending from the center
- Show a filled polygon connecting the skill values at 80, 65, 90, 70, 85 respectively, with hover revealing the exact score for each skill

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display pentagon-shaped radar chart structure                | major  | The pentagon shape is the foundation that holds all five skill axes in a radial layout.                          | None         |
| 2   | content     | Display "Coding" axis label                                  | minor  | This label identifies the first skill being measured on the radar chart.                                         | None         |
| 3   | content     | Display "Design" axis label                                  | minor  | This label identifies the second skill being measured.                                                           | None         |
| 4   | content     | Display "Communication" axis label                           | minor  | This label identifies the third skill being measured.                                                            | None         |
| 5   | content     | Display "Leadership" axis label                              | minor  | This label identifies the fourth skill being measured.                                                           | None         |
| 6   | content     | Display "Problem Solving" axis label                         | minor  | This label identifies the fifth skill being measured.                                                            | None         |
| 7   | layout      | Position axis labels extending from center point             | minor  | Radiating labels from center creates the classic radar chart spoke structure.                                    | None         |
| 8   | visual      | Display filled polygon connecting skill values               | major  | The filled polygon visualizes the overall skill profile shape for quick pattern recognition.                     | None         |
| 9   | state       | Plot Coding skill at value 80 on its axis                    | major  | Plotting 80 for Coding shows the proficiency level for that specific skill.                                      | None         |
| 10  | state       | Plot Design skill at value 65 on its axis                    | major  | Plotting 65 for Design shows a lower proficiency compared to other skills.                                       | None         |
| 11  | state       | Plot Communication skill at value 90 on its axis             | major  | Plotting 90 for Communication shows this is the strongest skill in the profile.                                  | None         |
| 12  | state       | Plot Leadership skill at value 70 on its axis                | major  | Plotting 70 for Leadership shows mid-level proficiency.                                                          | None         |
| 13  | state       | Plot Problem Solving skill at value 85 on its axis           | major  | Plotting 85 for Problem Solving shows high proficiency in this skill.                                            | None         |
| 14  | interaction | Display tooltip with exact score when hovering over skill    | major  | Hover tooltips let users see precise numeric values instead of estimating from the polygon shape.                | None         |

## Justification

The application achieved a 92.86% pass rate with one specific failure. A pentagon-shaped radar chart displays with five axes radiating from the center, labeled "Coding", "Design", "Communication", "Leadership", and "Problem Solving". A filled polygon connects the skill values, plotting Coding at 80, Design at 65, Communication at 90, Leadership at 70, and Problem Solving at 85. When hovering over any skill point on the polygon, a tooltip appears showing the exact numeric score for that skill. However, the model failed to position axis labels extending from the center point. Instead, labels appear at the outer edges of each axis or in a separate legend, not radiating from the center as required for proper radar chart structure. This positioning issue caused the failure despite all other functionality working correctly.
