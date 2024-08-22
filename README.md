# Drum Kit Project

This is a simple interactive drum kit web application built using HTML, CSS, and JavaScript. The project allows users to play different drum sounds by either clicking on the drum buttons or pressing the corresponding keys on the keyboard.

## Features

- Play drum sounds by clicking on the buttons on the webpage.
- Play drum sounds by pressing the corresponding keys (`w`, `a`, `s`, `d`, `j`, `k`, `l`) on the keyboard.
- Visual button animations when a drum sound is triggered.

## Code Overview

### HTML

The HTML file contains buttons representing different drum sounds. Each button has a class of `drum` and an inner text representing the corresponding keyboard key (`w`, `a`, `s`, `d`, `j`, `k`, `l`).

### CSS

The CSS file includes styles for the drum buttons and the pressed button animation.

### JavaScript

The JavaScript file handles the interaction logic. Here's a brief overview of the key functions:

- **Event Listeners:**  
  - Adds `click` event listeners to all drum buttons.
  - Adds a `keypress` event listener to detect keyboard presses.

- **makeSound(key):**  
  Plays the appropriate drum sound based on the key pressed or button clicked.  
  Uses the `Audio` object to play sound files located in the `sounds/` directory.

- **buttonAnimation(currentKey):**  
  Adds a visual "pressed" effect to the button associated with the key or click.  
  Removes the effect after a short delay using `setTimeout`.

## How to Run

1. Clone the repository or download the project files.
2. Ensure the project structure includes an `index.html`, a `styles.css`, a `sounds/` directory with the sound files (`tom-1.mp3`, `tom-2.mp3`, `tom-3.mp3`, `tom-4.mp3`, `snare.mp3`, `crash.mp3`, `kick-bass.mp3`), and a `script.js`.
3. Open the `index.html` file in your web browser.

## Project Structure

```plaintext
drum-kit/
│── images
├── index.html
├── styles.css
├── index.js
└── sounds/
    ├── tom-1.mp3
    ├── tom-2.mp3
    ├── tom-3.mp3
    ├── tom-4.mp3
    ├── snare.mp3
    ├── crash.mp3
    └── kick-bass.mp3
