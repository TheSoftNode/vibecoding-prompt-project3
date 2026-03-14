Category: Data_Visualization

Prompt style: Conversational

Title: Music Collection Relationship Visualizer

Prompt: I want to build a music collection tracker with visualization. Put a form at the top with inputs for Genre, Artist Name, and Music Title, along with an Add Entry button. When I add an entry, I want two visualizations to update automatically. On the left, show a relationship diagram with circles for each unique genre, artist, and song I've added, with lines connecting related items - like connecting Rock to Led Zeppelin to Stairway to Heaven. Below the form, show a bar chart displaying how many songs I have in each genre. When I click a genre bar, show me that genre's artists and songs in a details panel next to the chart. Preload with a few sample entries so I can see how it works right away.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display form with Genre, Artist Name, and Music Title inputs     | major  | The form provides the interface for users to input their music collection data.                           | None         |
| 2   | content     | Display Add Entry button                                         | minor  | The button triggers the action to save and visualize the new entry.                                       | None         |
| 3   | interaction | Save entry data when Add Entry button is clicked                 | major  | Saving entries builds the data collection that powers both visualizations.                                | C1, C2       |
| 4   | visual      | Display relationship diagram on the left side                    | major  | The diagram provides a visual map of how genres, artists, and songs connect.                              | None         |
| 5   | visual      | Show circles for each unique genre, artist, and song             | major  | Circles represent the individual entities in the music collection.                                        | C4           |
| 6   | visual      | Draw lines connecting related items in relationship diagram      | major  | Connection lines show the relationships between genres, artists, and specific songs.                      | C5           |
| 7   | interaction | Update relationship diagram when new entry is added              | major  | Live updates keep the diagram synchronized with the growing collection.                                   | C3, C4       |
| 8   | visual      | Display bar chart below the form                                 | major  | The bar chart provides a quantitative view of genre distribution.                                         | None         |
| 9   | state       | Calculate count of songs per genre                               | major  | Genre counts reveal which music categories dominate the collection.                                       | C3           |
| 10  | visual      | Display bars sized by song count for each genre                  | major  | Bar sizing allows visual comparison of genre popularity in the collection.                                | C9           |
| 11  | interaction | Update bar chart when new entry is added                         | major  | Live chart updates reflect the changing composition of the collection.                                    | C3, C8       |
| 12  | interaction | Filter to clicked genre when user clicks a bar                   | major  | Clicking enables users to drill down into a specific genre's details.                                     | C10          |
| 13  | content     | Display details panel beside the chart                           | minor  | The details panel provides space for showing filtered genre information.                                  | None         |
| 14  | content     | Show selected genre name in details panel                        | minor  | The genre name confirms which category's details are being displayed.                                     | C12, C13     |
| 15  | state       | Filter to show only clicked genre's artists and songs            | major  | Filtering isolates the specific artists and songs belonging to the selected genre.                        | C12          |
| 16  | content     | Display list of artists and songs for selected genre             | major  | Showing the filtered list gives users detailed information about that genre's contents.                   | C15          |
| 17  | content     | Preload form with sample music entries on initial load           | minor  | Sample data demonstrates the visualization's functionality immediately without requiring user input.      | None         |

## Justification

The Music Collection Relationship Visualizer achieved 53% pass rate (9/17 criteria) with failures in relationship diagram implementation and filtering logic. The form correctly displays three input fields for Genre, Artist Name, and Music Title (C1 passed) with an Add Entry button (C2 passed). When clicking Add Entry, the data saves successfully (C3 passed) and both visualizations update. The bar chart displays below the form (C8 passed) and correctly calculates song counts per genre (C9 passed), with bars sized proportionally - Rock with 3 songs appears taller than Jazz with 1 song (C10 passed). The bar chart updates live when new entries are added (C11 passed). However, the relationship diagram completely failed C4 and C5 - instead of displaying on the left side with circles for each unique entity, it rendered as a simple list in the center showing "Rock → Led Zeppelin → Stairway to Heaven" in text form without any circular nodes. The connection lines failed C6, appearing as plain arrows in the text rather than visual lines connecting circle nodes. Despite the diagram's structural failures, it did update when entries were added (C7 passed). Click interactions on the bar chart worked (C12 passed) and a details panel appeared beside the chart (C13 passed) showing the genre name (C14 passed), but the filtering logic failed C15 and C16 - when clicking the Rock bar, the details panel showed all artists and songs from the entire collection instead of filtering to only Rock's artists (Led Zeppelin, The Beatles) and songs (Stairway to Heaven, Hey Jude, Come Together). The preloaded sample data appeared on load (C17 passed) with 5 entries across Rock, Jazz, and Pop genres, allowing immediate demonstration of the visualization features.
