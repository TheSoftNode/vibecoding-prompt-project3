Category: Quick_Tools

Prompt style: Feature_List

Title: BMI Calculator with Category

Prompt: Build a BMI calculator with these features:
- Input fields for weight in kilograms and height in centimeters, then calculate BMI using the formula weight / (height/100)²
- Display the calculated BMI number and show a color-coded category: blue for "Underweight" (BMI < 18.5), green for "Normal" (18.5-24.9), yellow for "Overweight" (25-29.9), or red for "Obese" (30+)

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display input field for weight                               | major  | Weight input is one of the two required values for calculating BMI.                                              | None         |
| 2   | visual      | Display input field for height                               | major  | Height input is the second required value for calculating BMI.                                                   | None         |
| 3   | content     | Display label "Weight (kg)" for weight input                 | minor  | Labeling with units clarifies that weight should be entered in kilograms.                                        | None         |
| 4   | content     | Display label "Height (cm)" for height input                 | minor  | Labeling with units clarifies that height should be entered in centimeters.                                      | None         |
| 5   | state       | Calculate BMI using formula weight / (height/100)²           | major  | This is the standard BMI formula that produces the body mass index value.                                        | None         |
| 6   | content     | Display calculated BMI number                                | major  | Showing the numeric BMI value gives users their specific body mass index score.                                  | None         |
| 7   | state       | Determine category "Underweight" for BMI < 18.5              | major  | Categorizing as Underweight helps users understand if their BMI is below healthy range.                          | None         |
| 8   | state       | Determine category "Normal" for BMI 18.5-24.9                | major  | Categorizing as Normal tells users their BMI is in the healthy range.                                            | None         |
| 9   | state       | Determine category "Overweight" for BMI 25-29.9              | major  | Categorizing as Overweight indicates BMI is above healthy range but not obese.                                   | None         |
| 10  | state       | Determine category "Obese" for BMI 30+                       | major  | Categorizing as Obese indicates BMI is significantly above healthy range.                                        | None         |
| 11  | content     | Display category text for current BMI                        | major  | Showing the category name helps users interpret what their BMI number means.                                     | None         |
| 12  | visual      | Display category in blue color for "Underweight"             | minor  | Blue color provides visual coding for the underweight category.                                                  | None         |
| 13  | visual      | Display category in green color for "Normal"                 | minor  | Green color signals healthy BMI range.                                                                           | None         |
| 14  | visual      | Display category in yellow color for "Overweight"            | minor  | Yellow color warns of above-normal BMI.                                                                          | None         |
| 15  | visual      | Display category in red color for "Obese"                    | minor  | Red color alerts to high BMI level.                                                                              | None         |
| 16  | layout      | Position BMI result below the input fields                   | minor  | Placing results below inputs creates a top-to-bottom flow from data entry to calculated output.                  | None         |

## Justification

The application achieved a 93.75% pass rate with one specific failure. Two input fields labeled "Weight (kg)" and "Height (cm)" allow users to enter their measurements. The tool calculates BMI using the formula weight / (height/100)². The calculated BMI number displays along with a category determination: "Underweight" in blue for BMI < 18.5, "Normal" in green for BMI 18.5-24.9, "Overweight" in yellow for BMI 25-29.9, or "Obese" in red for BMI 30+. The category text appears with its corresponding color coding. However, the model failed to position the BMI result below the input fields. Instead, the result appears to the right of the inputs in a side-by-side layout, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
