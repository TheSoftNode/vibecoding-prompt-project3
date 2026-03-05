# UI/Landing Page

SaaS Landing Page with Interactive Pricing

## Prompt

Design a SaaS landing page that includes a hero section with a headline and call-to-action button, a features section with at least three feature cards, a testimonials section, and a pricing table with two plans. The pricing table must include a toggle that allows users to switch between Monthly and Annual pricing, and switching the toggle should update all displayed pricing values consistently. The primary pricing plan should be visually emphasized, and the CTA button in the hero section should reflect the currently selected pricing plan. All sections must be fully visible on initial page load.

## Rubric

| ID            | Description                                                                    | Weight | Rationale                                           | Dependent On  |
| ------------- | ------------------------------------------------------------------------------ | ------ | --------------------------------------------------- | ------------- |
| visual-1      | Render hero, features, testimonials, and pricing sections on initial page load | major  | All required sections must be present and visible.  | None          |
| content-1     | Include at least three feature cards in the features section                   | major  | The feature section must contain multiple entries.  | None          |
| content-2     | Display two pricing plans in the pricing section                               | major  | Two plans are explicitly required.                  | None          |
| interaction-1 | Allow toggling between Monthly and Annual pricing                              | major  | Users must be able to change pricing mode.          | None          |
| state-1       | Update all displayed pricing values when the toggle changes                    | major  | Pricing values must remain synchronized.            | interaction-1 |
| state-2       | Update the hero section CTA text to reflect the selected pricing plan          | major  | Cross-section coordination is required.             | interaction-1 |
| visual-2      | Visually distinguish the primary pricing plan from the secondary plan          | major  | Visual hierarchy must reflect plan emphasis.        | None          |
| layout-1      | Arrange pricing plans in a structured side-by-side or card layout              | minor  | Clear layout improves comparison and readability.   | None          |
| content-3     | Display at least two testimonial entries in the testimonials section           | minor  | Testimonials are explicitly required in the prompt. | None          |
