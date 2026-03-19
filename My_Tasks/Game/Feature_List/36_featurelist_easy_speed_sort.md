Category: Game

Prompt style: Feature_List

Title: Speed Sorter

Prompt: Build a number sorting challenge game with these features: Display five boxes arranged horizontally labeled "Box 1", "Box 2", "Box 3", "Box 4", "Box 5" from left to right. Display a "Start Round" button below the boxes. When players click "Start Round", generate 5 random numbers between 1 and 50 and display each number above its corresponding box. Display instruction text saying "Click boxes from smallest to largest number". When players click boxes, highlight clicked boxes in green in the order they were clicked. Display an attempts counter labeled "Attempts: 0" that increments each time "Start Round" is clicked. When all 5 boxes have been clicked, check if boxes were clicked in ascending order of their numbers. If the order is correct, display "Sorted Correctly!" in green text. If the order is wrong, display "Wrong Order!" in red text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display five boxes horizontally                      | major  | The boxes provide the sorting interface.                                                     | None         |
| 2   | content     | Label boxes "Box 1" through "Box 5" left to right    | major  | Labels identify each box position.                                                           | C1           |
| 3   | visual      | Display "Start Round" button below boxes             | major  | The button lets players begin a new sorting challenge.                                       | None         |
| 4   | state       | Generate 5 random numbers between 1 and 50           | major  | Random numbers create different sorting challenges.                                          | C3           |
| 5   | content     | Display each number above its corresponding box      | major  | Showing numbers tells players what values to sort.                                           | C4           |
| 6   | content     | Display "Click boxes from smallest to largest number" | major  | Instructions tell players the sorting rule.                                                  | None         |
| 7   | interaction | Highlight clicked boxes in green                     | major  | Green highlighting shows which boxes were clicked.                                           | C1           |
| 8   | state       | Track order boxes were clicked                       | major  | Recording order determines if the sort is correct.                                           | C7           |
| 9   | content     | Display attempts counter labeled "Attempts: 0"       | major  | The counter shows how many rounds the player has started.                                    | None         |
| 10  | state       | Increment attempts when "Start Round" clicked        | major  | Incrementing tracks the total number of sorting attempts.                                    | C3           |
| 11  | content     | Update displayed attempts count after increment      | major  | Updating display shows the current attempt number.                                           | C10          |
| 12  | state       | Detect when all 5 boxes clicked                      | major  | Checking completion determines when to evaluate the sort.                                    | C7           |
| 13  | state       | Check if boxes clicked in ascending number order     | major  | Checking order determines if the player sorted correctly.                                    | C8           |
| 14  | content     | Display "Sorted Correctly!" in green when correct    | major  | Green message confirms correct sorting.                                                      | C13          |
| 15  | content     | Display "Wrong Order!" in red when incorrect         | major  | Red message tells the player their sort was wrong.                                           | C13          |

## Justification

The speed sorter game works exactly as expected for number sorting challenges. Five boxes display horizontally labeled "Box 1" through "Box 5". A "Start Round" button displays below. Instruction text displays saying "Click boxes from smallest to largest number". An attempts counter labeled "Attempts: 0" displays on screen. When players click "Start Round", 5 random numbers between 1 and 50 generate and display above their boxes, and the attempts counter increments with the display updating. When players click boxes, they highlight in green in click order. When all 5 boxes are clicked, the click order is checked against ascending number order. If correct, "Sorted Correctly!" displays in green text. If wrong, "Wrong Order!" displays in red text.
