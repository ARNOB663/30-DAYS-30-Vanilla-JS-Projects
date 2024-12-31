# JavaScript Drum Kit

This project is part of the 30 Days 30 JS challenge. It is a fun and interactive drum kit built using vanilla JavaScript, HTML, and CSS. Users can play different drum sounds by pressing specific keys on their keyboard.

## How It Works

The drum kit consists of several keys, each associated with a different drum sound. When a user presses a key, the corresponding sound is played, and a visual effect is applied to the key.

### Key Features

- **Interactive Keys:** Each key on the drum kit is interactive and responds to user input.
- **Sound Effects:** Different drum sounds are played when the corresponding keys are pressed.
- **Visual Feedback:** Keys provide visual feedback when pressed, enhancing the user experience.

## Project Structure

- `index-FINISHED.html`: The main HTML file containing the structure of the drum kit.
- `style.css`: The CSS file for styling the drum kit.
- `sounds/`: A directory containing the audio files for the drum sounds.

## Code Explanation

### HTML

The HTML file defines the structure of the drum kit. Each key is represented by a `div` element with a `data-key` attribute corresponding to a specific key code. The audio files are linked using `audio` elements with matching `data-key` attributes.

### JavaScript

The JavaScript code handles the interaction logic:

- **removeTransition(e):** Removes the visual effect from the key after the transition ends.
- **playSound(e):** Plays the corresponding drum sound and adds a visual effect to the key when a key is pressed.
- **Event Listeners:** Listens for `keydown` events to trigger the `playSound` function and `transitionend` events to trigger the `removeTransition` function.

### CSS

The CSS file styles the drum kit and defines the visual effects applied to the keys when they are pressed.
