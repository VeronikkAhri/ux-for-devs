# 6. Accessibility Basics

Accessibility ensures that everyone, including people with disabilities, can use your application. Keep these guidelines in mind:

- **Provide text alternatives** for images, icons, and media so screen readers can describe them.
- **Use sufficient color contrast** between text and backgrounds to make content readable for users with low vision.
- **Support keyboard navigation** so all interactive elements can be reached without a mouse.
- **Label form fields clearly** and group related inputs to help users complete tasks without confusion.
- **Test with assistive technologies** like screen readers to verify your interface works for all users.

## Additional Tips

1. **Resize text gracefully.** Ensure layouts remain usable when users increase font size.
2. **Avoid relying solely on color** to convey information—use icons or text as well.
3. **Provide captions and transcripts** for videos and audio clips.
4. **Announce dynamic content** (like modals) so screen readers know something has changed.
5. **Give controls clear focus styles** to indicate where keyboard users are on the page.

Building accessibility into your workflow leads to products that are inclusive and easier for everyone to use. It may take more effort upfront, but the benefits reach a much wider audience.

## Testing Tips

- Run automated tools like axe or Lighthouse to catch basic contrast and labeling errors.
- Include users with disabilities in your usability tests to uncover real-world barriers.
- Review error messages and notifications for screen reader compatibility.

## Common Issues to Watch For

1. **Missing alt text** on decorative images that still get focus.
2. **Keyboard traps** where users cannot tab away from a modal or menu.
3. **Lack of ARIA roles** for custom widgets such as sliders or dropdowns.
4. **Inconsistent heading order** that makes it hard to skim with assistive tech.

Remember: accessibility is an ongoing process. Revisit these steps whenever you introduce new components or features.
