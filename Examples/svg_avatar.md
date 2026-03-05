SVG Avatar
Example SVG Avatar
Difficulty
Medium
Category
Game
Style
Detailed Specification
Length
Detailed
Prompt
Can you make me an avatar generator? I want to pick face shape, eyes, mouth, hair and colors. Preview as SVG with download button.

**Difficulty: Medium**

| ID            | Description                                                      | Weight | Rationale                                                                             | Dependent On |
| ------------- | ---------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------- | ------------ |
| visual-1      | Render avatar preview using SVG elements                         | major  | SVG provides scalable, resolution-independent rendering ideal for avatar generation.  | None         |
| content-1     | Display a selector for face shape                                | major  | Face shape is the foundational element of an avatar, essential for personalization.   | None         |
| content-2     | Display a selector for eye style                                 | major  | Eye style significantly impacts avatar expressiveness and identity.                   | None         |
| content-3     | Display a selector for mouth style                               | major  | Mouth style contributes to the avatar's expression and personality.                   | None         |
| content-4     | Display a selector for hair style                                | major  | Hair style is one of the most recognizable features for distinguishing avatars.       | None         |
| visual-2      | Display a color picker or selector for skin tone                 | minor  | Skin tone selection is fundamental for creating inclusive and representative avatars. | None         |
| visual-3      | Display a color picker or selector for hair color                | minor  | Hair color adds an important layer of visual personalization to the avatar.           | None         |
| interaction-1 | Update avatar SVG preview when any option is changed             | major  | Real-time feedback is essential for iterative customization UX.                       | visual-1     |
| interaction-2 | Download a valid SVG file when the user clicks the export button | major  | SVG export enables users to save and reuse their custom avatar across applications.   | None         |
| layout-1      | Display avatar preview adjacent to customization controls        | minor  | Keeping controls near the preview allows users to see changes while adjusting.        | None         |

Difficulty: Medium
ID
Description
Weight
Rationale
Dependent On
visual-1
Render avatar preview using SVG elements
major
SVG provides scalable, resolution-independent rendering ideal for avatar generation.
None
content-1
Display a selector for face shape
major
Face shape is the foundational element of an avatar, essential for personalization.
None
content-2
Display a selector for eye style
major
Eye style significantly impacts avatar expressiveness and identity.
None
content-3
Display a selector for mouth style
major
Mouth style contributes to the avatar's expression and personality.
None
content-4
Display a selector for hair style
major
Hair style is one of the most recognizable features for distinguishing avatars.
None
visual-2
Display a color picker or selector for skin tone
minor
Skin tone selection is fundamental for creating inclusive and representative avatars.
None
visual-3
Display a color picker or selector for hair color
minor
Hair color adds an important layer of visual personalization to the avatar.
None
interaction-1
Update avatar SVG preview when any option is changed
major
Real-time feedback is essential for iterative customization UX.
visual-1
interaction-2
Download a valid SVG file when the user clicks the export button
major
SVG export enables users to save and reuse their custom avatar across applications.
None
layout-1
Display avatar preview adjacent to customization controls
minor
Keeping controls near the preview allows users to see changes while adjusting.
None
