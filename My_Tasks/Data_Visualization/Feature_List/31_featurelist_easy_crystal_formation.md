Category: Data_Visualization

Prompt style: Feature_List

Title: Crystal Formation Tracker

Prompt: Build a crystal formation tracker that visualizes formation speed against stability limits. Display 5 vertical crystals representing Quartz, Amethyst, Citrine, Topaz, Emerald, with realistic sample formation rates in millimeters per hour. Load initial formation data showing varied crystal growth speeds, with at least one crystal meeting and at least one exceeding the 8 mm/h stability threshold. Color crystals that stayed within the threshold (8 or fewer mm/h) in cyan and crystals that exceeded the threshold in magenta. When users click any crystal, that crystal displays a shield icon at the top if it stayed within the threshold, or a crack icon if it exceeds the threshold.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                        | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | layout      | Display 5 vertical crystals                                                        | major  | Users need crystals as the visual containers for displaying formation rates.        | None         |
| 2   | content     | Display crystal names Quartz, Amethyst, Citrine, Topaz, Emerald                    | major  | Crystal names help users identify which crystal each represents.                    | None         |
| 3   | state       | Load initial formation data with varied growth speeds                              | major  | Loading formation data initializes the crystal values for visualization.            | None         |
| 4   | state       | Load data with at least one crystal meeting and at least one exceeding 8 mm/h threshold | major  | Mixed data ensures both cyan and magenta crystals are visible for comparison.       | None         |
| 5   | content     | Display realistic sample formation rates in millimeters per hour                    | major  | Realistic formation rates provide believable crystal growth data.                   | C3           |
| 6   | visual      | Color crystals with 8 or fewer mm/h cyan                                           | major  | Cyan color helps users quickly identify crystals that stayed within the 8 mm/h threshold. | C1, C4       |
| 7   | visual      | Color crystals above 8 mm/h magenta                                                | major  | Magenta color helps users spot crystals that exceeded the 8 mm/h threshold.         | C1, C4       |
| 8   | interaction | Display a shield icon at the top if the crystal stayed within the threshold when clicked | major  | The shield icon confirms that the crystal successfully stayed within the stability threshold. | None         |
| 9   | interaction | Display the crack icon at the top if the crystal exceeds the threshold when clicked | major  | The crack icon indicates the crystal exceeded the stability threshold.              | None         |

## Justification

The crystal formation tracker works exactly as expected for visualizing crystal formation with stability indicators. Five vertical crystals display representing Quartz, Amethyst, Citrine, Topaz, Emerald with realistic sample formation rates in millimeters per hour. Initial formation data loads with varied growth speeds showing at least one crystal meeting and at least one crystal exceeding the 8 mm/h stability threshold. Crystals with 8 or fewer mm/h display in cyan color while crystals above 8 mm/h display in magenta color. When users click any crystal, that crystal displays a shield icon at the top if it stayed within the threshold or a crack icon if it exceeds the threshold.
