# Day20
## Text-to-Speech Converter

A simple **Text-to-Speech Converter** built using HTML, CSS, and JavaScript. This web app allows users to convert their input text into speech with adjustable speech rate and pitch.

## Features

- Input any text to be converted into speech.
- Choose from different available voices (if supported by the browser).
- Adjust the speech rate (speed of the voice).
- Adjust the pitch (tone of the voice).
- Simple and intuitive interface.

## Technologies Used

- **HTML**: Used for creating the structure of the webpage.
- **CSS**: Used for styling the interface.
- **JavaScript**: Used for logic and functionality, including speech synthesis.

## How to Use

1. Open the `index.html` file in your browser.
2. Type the text you want to convert into speech into the text input field.
3. Adjust the voice rate and pitch sliders if necessary.
4. Click on the **Speak** button to hear the text being spoken.

## Example Code

Here’s a basic example of the JavaScript functionality using the Web Speech API:

```javascript
const synth = window.speechSynthesis;
const speakButton = document.getElementById('speak');
const textInput = document.getElementById('text-input');

speakButton.addEventListener('click', () => {
  const utterance = new SpeechSynthesisUtterance(textInput.value);
  synth.speak(utterance);
});
