# JS and CSS Clock

This project is part of the 30 Days 30 JS challenge. It is a real-time clock built using vanilla JavaScript and CSS. The clock displays the current time with hour, minute, and second hands, and updates every second.

## How It Works

The clock consists of three hands (hour, minute, and second) that rotate to indicate the current time. The positions of the hands are updated every second using JavaScript.

### Key Features

- **Real-Time Updates:** The clock updates every second to display the current time.
- **Smooth Transitions:** The hands of the clock move smoothly thanks to CSS transitions.
- **Responsive Design:** The clock is styled to be visually appealing and responsive.

## Project Structure

- `index-FINISHED.html`: The main HTML file containing the structure of the clock and the embedded CSS and JavaScript.

## Code Explanation

### HTML

The HTML file defines the structure of the clock. The clock face and hands are represented by `div` elements with appropriate classes.

### CSS

The CSS styles the clock and defines the visual appearance of the clock face and hands. It also includes transitions for smooth movement of the hands.

### JavaScript

The JavaScript code handles the logic for updating the positions of the clock hands:

- **setDate():** Calculates the current time and updates the rotation of the clock hands accordingly.
- **setInterval(setDate, 1000):** Calls the `setDate` function every second to update the clock.

