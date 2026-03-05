Shopping App
Shopping App
Difficulty
Medium
Category
Web Application
Style
Feature List
Length
Moderate
Prompt
Create a shopping app with a nav bar containing two links: Products and Cart. The app should display either the Products page or the Cart page when their links are clicked. Products page: product grid (title, price, image) and a detailed view of the selected (title, price, image, description, rating) item with quantity input and an Add to Cart button. Cart page: added items (title, price, image, description, rating) with Remove buttons, and a Checkout link. Use mock jeans data.
Required Libraries
vanilla-js react-js

Rubric

| ID            | Description                                                                                   | Weight | Rationale                                                                                       | Dependent On         |
| ------------- | --------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------- | -------------------- |
| visual-1      | Render a navigation bar with two links                                                        | major  | The navigation bar is essential for navigating between the Products and Cart pages.             | None                 |
| visual-2      | Display an input labeled "quantity" in a product's detailed view                              | major  | Quantity selection allows users to add multiple items of the same product to their cart.        | content-2            |
| interaction-1 | Display a Products page when a Products link is clicked                                       | major  | Confirms navigation and display logic for the Products page.                                    | visual-1             |
| interaction-2 | Display a Cart page when a Cart link is clicked                                               | major  | The Cart page is where users review all products they intend to purchase.                       | visual-1             |
| state-1       | Create an object containing mock jeans data with title, price, image, description, and rating | major  | These product attributes form the core data model for a jeans shopping application.             | None                 |
| content-1     | Create a product grid displaying title, price, and image for each product                     | major  | The product grid provides an overview of all available products for browsing.                   | None                 |
| content-2     | Create a detailed view displaying title, price, image, description, and rating of a product   | major  | The detailed view provides comprehensive product information for informed purchasing decisions. | None                 |
| interaction-3 | Change the detailed view text when a different product grid item is clicked                   | major  | Updating the detailed view on selection demonstrates proper selected-item state management.     | content-1, content-2 |
| interaction-4 | Add a product to a cart when an Add to Cart button is clicked                                 | major  | Adding products to the cart is the core shopping interaction.                                   | None                 |
| content-4     | Create a Cart page displaying title, price, image, description, and rating for each product   | major  | The Cart page allows users to review added products before checkout.                            | None                 |
| interaction-5 | Remove a product from a cart when a Remove button is clicked                                  | major  | Removing products gives users control over their shopping selections.                           | None                 |
| content-5     | Display a Checkout link in a Cart page                                                        | minor  | A Checkout link provides the expected next step in the shopping workflow.                       | None                 |

ID
Description
Weight
Rationale
Dependent On
visual-1
Render a navigation bar with two links
major
The navigation bar is essential for navigating between the Products and Cart pages.
None
visual-2
Display an input labeled "quantity" in a product's detailed view
major
Quantity selection allows users to add multiple items of the same product to their cart.
content-2
interaction-1
Display a Products page when a Products link is clicked
major
Confirms navigation and display logic for the Products page.
visual-1
interaction-2
Display a Cart page when a Cart link is clicked
major
The Cart page is where users review all products they intend to purchase.
visual-1
state-1
Create an object containing mock jeans data with title, price, image, description, and rating
major
These product attributes form the core data model for a jeans shopping application.
None
content-1
Create a product grid displaying title, price, and image for each product
major
The product grid provides an overview of all available products for browsing.
None
content-2
Create a detailed view displaying title, price, image, description, and rating of a product
major
The detailed view provides comprehensive product information for informed purchasing decisions.
None
interaction-3
Change the detailed view text when a different product grid item is clicked
major
Updating the detailed view on selection demonstrates proper selected-item state management.
content-1, content-2
interaction-4
Add a product to a cart when an Add to Cart button is clicked
major
Adding products to the cart is the core shopping interaction.
None
content-4
Create a Cart page displaying title, price, image, description, and rating for each product
major
The Cart page allows users to review added products before checkout.
None
interaction-5
Remove a product from a cart when a Remove button is clicked
major
Removing products gives users control over their shopping selections.
None
content-5
Display a Checkout link in a Cart page
minor
A Checkout link provides the expected next step in the shopping workflow.
None
