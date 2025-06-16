# 5. Examples and Exercises

The best way to learn UX is by doing. The examples below show how to apply principles from this course.

## Example: Button Feedback

```html
<button class="action">Save</button>
```

Provide immediate feedback when the button is clicked:

```javascript
const button = document.querySelector('.action');
button.addEventListener('click', () => {
  button.textContent = 'Saved!';
});
```

## Example: Accessible Form

```html
<form aria-label="Contact form">
  <label for="email">Email</label>
  <input id="email" type="email" required />
  <button type="submit">Send</button>
</form>
```

This markup ensures screen readers understand the purpose of each field and the form itself.

## Example: Clear Error Messaging

```javascript
const form = document.querySelector('form');
form.addEventListener('submit', (e) => {
  const email = form.querySelector('#email');
  if (!email.value) {
    e.preventDefault();
    alert('Please enter an email address.');
  }
});
```

Explicit error messages guide users toward completing tasks successfully.

## Example: Responsive Layout

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
.item {
  flex: 1 1 200px;
}
```

Flexbox lets the interface adapt to different screen sizes so content stays usable on mobile and desktop.

## Example: Progress Indicator

```html
<progress value="32" max="100">32%</progress>
```

Use a progress bar when tasks take more than a couple of seconds. It sets the right expectations for users.

## Example: Dark Mode Toggle

```html
<button id="toggle-theme">Switch Theme</button>
```

```javascript
const button = document.getElementById('toggle-theme');
button.addEventListener('click', () => {
  document.body.classList.toggle('dark');
});
```

This feature taps into a current trend. Many people prefer darker UIs, especially at night.

## Example: Loading Skeleton

```html
<div class="card loading">
  <div class="placeholder title"></div>
  <div class="placeholder text"></div>
</div>
```

```css
.loading .placeholder {
  background: #eee;
  animation: pulse 1s infinite ease-in-out;
}
```

Skeleton screens let users know content is on the way and improve the perception of speed.

## Example: Inline Form Validation

```javascript
const input = document.getElementById('email');
input.addEventListener('blur', () => {
  if (!input.validity.valid) {
    input.classList.add('error');
    input.setAttribute('aria-describedby', 'email-error');
  }
});
```

```html
<span id="email-error" class="error-message">Please enter a valid email address.</span>
```

Inline validation helps users fix mistakes immediately, reducing frustration.

## Exercise

Pick a feature in your own project and improve its UX using what you've learned. Focus on clarity, feedback, and accessibility. Share your code with a friend or colleague and ask for their thoughts.

## Example: Accessible Modal Dialog

```html
<button id="open-dialog">Info</button>
<div id="modal" role="dialog" aria-modal="true" hidden>
  <p>This dialog describes a critical update.</p>
  <button id="close-dialog">Close</button>
</div>
```

```javascript
const modal = document.getElementById('modal');
const openBtn = document.getElementById('open-dialog');
const closeBtn = document.getElementById('close-dialog');
openBtn.addEventListener('click', () => {
  modal.hidden = false;
  modal.focus();
});
closeBtn.addEventListener('click', () => {
  modal.hidden = true;
  openBtn.focus();
});
```

Using `role="dialog"` and returning focus to the trigger ensures assistive technology users aren’t trapped inside the modal.

## Example: Sticky Header

```css
header {
  position: sticky;
  top: 0;
  background: #fff;
  border-bottom: 1px solid #ccc;
}
```

A sticky header keeps key navigation visible as users scroll long pages.

## Example: Live Region Updates

```html
<div id="status" aria-live="polite"></div>
```

```javascript
function announce(message) {
  const status = document.getElementById('status');
  status.textContent = message;
}
```

Live regions provide dynamic notifications without interrupting screen reader users.

## Additional Exercise

Refactor an existing component in your project to improve keyboard support. Document the before-and-after behavior and note any challenges you encountered.

## Example: Accessible Table

```html
<table aria-label="Schedule">
  <thead>
    <tr><th>Time</th><th>Activity</th></tr>
  </thead>
  <tbody>
    <tr><td>9 AM</td><td>Check email</td></tr>
    <tr><td>10 AM</td><td>Team stand-up</td></tr>
  </tbody>
</table>
```

Tables convey structured information to screen readers when you provide header and body elements.

## Example: Reduced Motion

```css
@media (prefers-reduced-motion: reduce) {
  .spinner {
    animation: none;
  }
}
```

Respecting the `prefers-reduced-motion` setting ensures users who are sensitive to animation can still enjoy your site.

## Exercise: Design a Simple Game Interface

Sketch out controls for a puzzle game that can be played with keyboard, mouse, or touch. Focus on clear icons, high contrast, and straightforward instructions. Share your design with friends and gather feedback on its clarity.
