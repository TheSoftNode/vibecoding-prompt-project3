Category: Data_Visualization

Prompt style: Conversational

Title: Customer Journey Chord Diagram

Prompt: I want to build a customer journey visualization showing how users move between five touchpoints using a chord diagram. Arrange touchpoints around a circle with ribbons connecting them - ribbon widths match user flow volumes. Flows are directional. When I click a touchpoint, filter to show only its connected ribbons and update a stats panel showing total users coming in, going out, and the net difference - color that green if positive, red if negative. Small flows get grouped as "Low Traffic". Preload with sample customer journey data.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display five touchpoint arcs evenly spaced around circle         | major  | Even spacing creates a balanced circular layout for visualizing customer journey flows.                   | None         |
| 2   | content     | Label touchpoints as Website, Email, Social Media, Store, Phone Support | minor  | Labels help users identify which arc represents each customer touchpoint.                                 | None         |
| 3   | visual      | Draw curved ribbons connecting touchpoints                       | major  | Curved ribbons distinguish chord diagrams from simple network graphs and improve aesthetics.              | C1           |
| 4   | state       | Size ribbon width proportional to flow volume                    | major  | Proportional widths allow users to compare flow volumes visually without reading exact numbers.           | None         |
| 5   | state       | Treat flows as directional (Website→Email ≠ Email→Website)       | major  | Directional flows accurately represent one-way customer journey paths rather than bidirectional links.    | None         |
| 6   | state       | Group flows under 50 users into single ribbon                    | major  | Grouping minor flows reduces visual clutter while preserving data completeness.                           | C4           |
| 7   | visual      | Display "Low Traffic" ribbon as thin dashed line                 | minor  | The dashed style visually distinguishes grouped minor flows from individual major flows.                  | C6           |
| 8   | layout      | Position ribbons to not overlap touchpoint arcs                  | minor  | Avoiding overlaps ensures touchpoint labels remain readable and the diagram stays clean.                  | C1, C3       |
| 9   | interaction | Filter view to show only connected ribbons when touchpoint clicked | major  | Filtering reduces visual complexity and lets users focus on one touchpoint's journey patterns.            | None         |
| 10  | content     | Display stats panel on the right when touchpoint clicked         | minor  | Right-side placement keeps stats visible without covering the main diagram.                               | C9           |
| 11  | content     | Show touchpoint name in stats panel                              | minor  | The name confirms which touchpoint's statistics are being displayed.                                      | C10          |
| 12  | state       | Calculate total inbound flow (sum of flows INTO touchpoint)      | major  | Inbound totals show how many customers arrive at this touchpoint from others.                             | C5           |
| 13  | state       | Calculate total outbound flow (sum of flows OUT of touchpoint)   | major  | Outbound totals show how many customers leave this touchpoint for others.                                 | C5           |
| 14  | content     | Display inbound and outbound flow totals in stats panel          | major  | Displaying both totals gives users a complete picture of the touchpoint's journey role.                   | C12, C13     |
| 15  | state       | Calculate net flow as inbound minus outbound                     | major  | Net flow reveals whether a touchpoint is a destination (positive) or waypoint (negative).                 | C12, C13     |
| 16  | visual      | Color net flow green if positive, red if negative                | major  | Color coding provides instant visual feedback about the touchpoint's role in customer journeys.           | C15          |

## Justification

The Customer Journey Chord Diagram achieved 50% pass rate (8/16 criteria) with failures in directionality and calculations. The visualization correctly displays five touchpoint arcs evenly spaced around a circle (C1 passed) labeled Website, Email, Social Media, Store, and Phone Support (C2 passed) with curved ribbons connecting them (C3 passed). However, the ribbon width calculation failed C4 - instead of being proportional to flow volumes, all ribbons appeared roughly equal thickness, making it impossible to distinguish Website→Email (120 users) from Store→Phone Support (90 users) visually. The model completely failed C5 by treating flows as bidirectional - it drew a single ribbon between Website and Email representing the sum of both directions (160 users) instead of two separate directional ribbons for Website→Email (120) and Email→Website (40). This fundamental error cascaded through the calculations. The grouping logic failed C6 and C7 - flows under 50 users (Social Media→Store with 50 users, Phone Support→Store with 30 users) were drawn as individual solid ribbons instead of being grouped into a single dashed "Low Traffic" ribbon. Ribbon positioning worked correctly, avoiding touchpoint arc overlaps (C8 passed). Click interactions functioned: clicking a touchpoint filtered to show only connected ribbons (C9 passed) and displayed a stats panel on the right (C10 passed) with the touchpoint name (C11 passed). However, the inbound/outbound calculations failed C12 and C13 due to the bidirectional flow error - clicking Store showed inbound as 280 (Website 80 + Email 150 + Social Media 50) but should exclude Phone Support→Store's 30 since that was grouped. The net flow calculation failed C15, showing -60 instead of the correct value, and the color coding failed C16 by always displaying green regardless of whether net flow was actually positive or negative.
