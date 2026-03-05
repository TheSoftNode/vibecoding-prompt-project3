# Weather Dashboard

## Prompt

Build a weather dashboard.

## Rubric

| ID        | Description                                                                                                   | Weight | Rationale                                                                      | Dependent On |
| --------- | ------------------------------------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| visual-1  | Display a weather dashboard with a clearly defined current conditions section and a separate forecast section | major  | A dashboard must show structured sections to be considered complete.           | None         |
| state-1   | Provide mock weather data in code for current conditions and forecast                                         | major  | Preloaded data ensures the dashboard is evaluable on initial render.           | None         |
| content-1 | Display a current temperature value sourced from the mock data                                                | major  | Temperature is a core weather attribute.                                       | state-1      |
| content-2 | Display a current weather condition label sourced from the mock data                                          | major  | Condition text is required for meaning.                                        | state-1      |
| content-3 | Display at least three forecast entries showing a time label and temperature                                  | major  | A forecast section is required to satisfy reasonable dashboard expectations.   | state-1      |
| visual-2  | Present forecast entries as visually distinct rows or blocks                                                  | minor  | Forecast entries must be visually separable for readability.                   | None         |
| layout-1  | Position the current conditions section above or beside the forecast section                                  | minor  | Clear structural arrangement improves interpretability.                        | None         |
| state-2   | Avoid external API calls and rely solely on static mock data                                                  | major  | The task must remain fully client-side and evaluable from code and screenshot. | None         |
