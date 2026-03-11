Category: Data_Visualization

Prompt style: Feature_List

Title: Skill Radar Chart

Prompt: Build a radar chart showing skill proficiency. Display a pentagon-shaped radar chart with 5 axes labeled "Coding", "Design", "Communication", "Leadership", "Problem Solving", each extending from the center. Show a filled polygon connecting the skill values at 80, 65, 90, 70, 85 respectively, with hover revealing the exact score for each skill.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display pentagon-shaped radar chart structure                | major  | The pentagon shape creates the five-sided structure needed for plotting five different skills.                   | None         |
| 2   | content     | Display "Coding" axis label                                  | minor  | Users need to know which axis represents coding skills.                                                          | None         |
| 3   | content     | Display "Design" axis label                                  | minor  | Users need to know which axis represents design skills.                                                          | None         |
| 4   | content     | Display "Communication" axis label                           | minor  | Users need to know which axis represents communication skills.                                                   | None         |
| 5   | content     | Display "Leadership" axis label                              | minor  | Users need to know which axis represents leadership skills.                                                      | None         |
| 6   | content     | Display "Problem Solving" axis label                         | minor  | Users need to know which axis represents problem solving skills.                                                 | None         |
| 7   | layout      | Position axis labels extending from center point             | minor  | Labels radiating from the center match the standard radar chart layout.                                          | None         |
| 8   | visual      | Display filled polygon connecting skill values               | major  | The filled polygon shows the overall skill profile at a glance.                                                  | None         |
| 9   | content     | Plot Coding skill at value 80 on its axis                    | major  | The value 80 shows the coding proficiency level.                                                                 | None         |
| 10  | content     | Plot Design skill at value 65 on its axis                    | major  | The value 65 shows the design proficiency level.                                                                 | None         |
| 11  | content     | Plot Communication skill at value 90 on its axis             | major  | The value 90 shows the communication proficiency level.                                                          | None         |
| 12  | content     | Plot Leadership skill at value 70 on its axis                | major  | The value 70 shows the leadership proficiency level.                                                             | None         |
| 13  | content     | Plot Problem Solving skill at value 85 on its axis           | major  | The value 85 shows the problem solving proficiency level.                                                        | None         |
| 14  | interaction | Display tooltip with exact score when hovering over skill    | major  | Hover tooltips give users the precise number without having to estimate from the chart.                          | None         |

## Justification

The application achieved a 92.86% pass rate with one specific failure. A pentagon-shaped radar chart displays with five axes radiating from the center, labeled "Coding", "Design", "Communication", "Leadership", and "Problem Solving". A filled polygon connects the skill values, plotting Coding at 80, Design at 65, Communication at 90, Leadership at 70, and Problem Solving at 85. When hovering over any skill point on the polygon, a tooltip appears showing the exact numeric score for that skill. However, the model failed to position axis labels extending from the center point. Instead, labels appear at the outer edges of each axis or in a separate legend, not radiating from the center as required for proper radar chart structure. This positioning issue caused the failure despite all other functionality working correctly.
