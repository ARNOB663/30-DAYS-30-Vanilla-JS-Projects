# CSS Variables and JS

This project is part of the 30 Days 30 JS challenge. It demonstrates how to update CSS variables dynamically using JavaScript. The project includes a simple interface with controls to adjust the padding, blur effect, and background color of an image in real-time.

## How It Works

The project consists of three controls:
- **Spacing:** Adjusts the padding around the image.
- **Blur:** Adjusts the blur effect applied to the image.
- **Base Color:** Changes the background color of the image and the highlight color of the text.

### Key Features

- **Real-Time Updates:** The CSS variables are updated in real-time as the user interacts with the controls.
- **Responsive Design:** The project is styled to be visually appealing and responsive.

## Project Structure

- `index-FINISHED.html`: The main HTML file containing the structure of the project, embedded CSS, and JavaScript.

## Code Explanation

### HTML

The HTML file defines the structure of the project, including the controls and the image.

### CSS

The CSS defines the styles for the project, including the CSS variables. The variables are used to control the padding, blur effect, and background color of the image.

### JavaScript

The JavaScript code handles the logic for updating the CSS variables based on user input. It listens for `change` and `mousemove` events on the input elements and updates the corresponding CSS variables.

```javascript
// filepath: /c:/30-DAYS-30-Vanilla-JS-Projects/03 - CSS Variables/index-FINISHED.html

<script>
  const inputs = document.querySelectorAll('.controls input');

  function handleUpdate() {
    const suffix = this.dataset.sizing || '';
    document.documentElement.style.setProperty(`--${this.name}`, this.value + suffix);
  }

  inputs.forEach(input => input.addEventListener('change', handleUpdate));
  inputs.forEach(input => input.addEventListener('mousemove', handleUpdate));
</script>