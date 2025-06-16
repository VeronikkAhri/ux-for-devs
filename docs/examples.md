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

This markup ensures screen readers understand the purpose of each field and the
form itself.

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

Flexbox lets the interface adapt to different screen sizes so content stays
usable on mobile and desktop.

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

## Exercise

Pick a feature in your own project and improve its UX using what you've learned. Focus on clarity, feedback, and accessibility.
