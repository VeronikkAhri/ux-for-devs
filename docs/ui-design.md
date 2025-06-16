# 12. UI Design Fundamentals

Creating visually appealing interfaces goes hand in hand with delivering great UX. This lesson focuses on key UI design concepts that complement the principles covered earlier in the course.

## Visual Hierarchy

Arrange elements so users notice the most important items first. Use size, color, and spacing to guide the eye naturally across the page. Avoid clutter by grouping related controls and separating them from secondary actions.

## Typography

- Choose fonts that are legible at various sizes.
- Limit the number of typefaces to maintain consistency.
- Use hierarchy in headings and body text to break up long sections.

```css
body {
  font-family: system-ui, sans-serif;
  line-height: 1.5;
}
```

## Color and Contrast

Establish a color palette that supports your brand while providing sufficient contrast for readability. Tools like contrast checkers help verify that text is easy to read against its background.

## Layout and Spacing

Consistent spacing makes interfaces feel intentional. Define a scale of spacing units—such as 4px, 8px, and 16px—and apply them throughout your layouts. Use grids or flexbox to keep components aligned.

## Iconography

Icons can clarify meaning when used carefully. Pair icons with labels to prevent confusion and keep the style consistent by reusing a single icon set.

## States and Transitions

Plan for various UI states like hover, active, and disabled. Subtle transitions help users recognize changes without feeling disoriented. Keep animations short and respect the `prefers-reduced-motion` setting.

## Writing Microcopy

Short labels and helper text improve clarity. Use verbs to indicate actions ("Save", "Upload") and keep error messages informative but polite.

## Responsive Design

Design layouts that adapt to different screen sizes using flexible grids and media queries. Prioritize content so mobile users can accomplish core tasks with minimal scrolling.

## Prototyping Tools

Sketch your ideas using paper, design software, or simple code prototypes. Tools like Figma or Penpot allow you to share layouts quickly and gather feedback before development begins.

## Putting It All Together

UI design is iterative—expect to refine colors, spacing, and wording over time. Keep your users' needs at the center of each decision, test frequently, and document your rationale so future team members understand why things look and behave the way they do.

