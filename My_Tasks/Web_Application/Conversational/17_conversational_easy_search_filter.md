Category: Web_Application

Prompt style: Conversational

Title: Live Search Filter

Prompt: I need a live search filter for a product list. Display 8 product cards showing name and price: "Laptop $999", "Mouse $25", "Keyboard $75", "Monitor $299", "Headphones $150", "Webcam $80", "Speaker $120", "Microphone $65". Show a search input at the top labeled "Search products". As I type in the search box, filter the visible cards in real-time to show only products whose names contain the search text, hiding non-matching cards.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display search input field                                   | major  | The search input is where users enter their filter query.                                                        | None         |
| 2   | content     | Display label "Search products" on input                     | minor  | Labeling clarifies the search function for filtering products.                                                   | None         |
| 3   | layout      | Position search input at the top                             | minor  | Top positioning creates a standard search-then-results layout.                                                   | None         |
| 4   | visual      | Display 8 product cards                                      | major  | Product cards are the items being filtered by the search.                                                        | None         |
| 5   | content     | Display "Laptop $999" on first card                          | minor  | This card provides one of the searchable products with name and price.                                           | None         |
| 6   | content     | Display "Mouse $25" on second card                           | minor  | This card provides another searchable product.                                                                   | None         |
| 7   | content     | Display "Keyboard $75" on third card                         | minor  | This card provides another searchable product.                                                                   | None         |
| 8   | content     | Display "Monitor $299" on fourth card                        | minor  | This card provides another searchable product.                                                                   | None         |
| 9   | content     | Display "Headphones $150" on fifth card                      | minor  | This card provides another searchable product.                                                                   | None         |
| 10  | content     | Display "Webcam $80" on sixth card                           | minor  | This card provides another searchable product.                                                                   | None         |
| 11  | content     | Display "Speaker $120" on seventh card                       | minor  | This card provides another searchable product.                                                                   | None         |
| 12  | content     | Display "Microphone $65" on eighth card                      | minor  | This card provides another searchable product.                                                                   | None         |
| 13  | state       | Store current search text from input                         | major  | Storing search text is necessary to compare against product names for filtering.                                 | None         |
| 14  | state       | Filter products to show only matching names                  | major  | Filtering logic determines which cards should be visible based on the search query.                              | None         |
| 15  | interaction | Update visible cards in real-time as search text changes     | major  | Real-time filtering provides instant feedback as users type, showing results without waiting for enter/submit.   | C1           |
| 16  | visual      | Hide cards that don't match search text                      | major  | Hiding non-matching cards focuses attention on relevant results.                                                 | None         |
| 17  | layout      | Position product cards below the search input                | minor  | Placing cards below the search creates a top-to-bottom flow from filter control to filtered results.            | None         |

## Justification

The application achieved a 94.12% pass rate with one specific failure. A search input labeled "Search products" displays at the top. Below it, 8 product cards show: "Laptop $999", "Mouse $25", "Keyboard $75", "Monitor $299", "Headphones $150", "Webcam $80", "Speaker $120", "Microphone $65". The tool stores the current search text from the input. As users type, it filters products to show only cards whose names contain the search text. Visible cards update in real-time as the search text changes, and non-matching cards are hidden from view. However, the model failed to position product cards below the search input. Instead, cards appear to the right of the search in a side panel or above it with search at the bottom, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
