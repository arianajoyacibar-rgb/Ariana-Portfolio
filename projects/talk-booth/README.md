# Talk Booth

Make a mascot talk in the browser. Inspired by the idea behind Zeke & Learn's Mascot Booth, with its own code.

## Features
- Upload any mascot image, or use the built-in sample
- Type a script and pick a voice (Web Speech API), with pitch and speed controls
- Speech events drive a squash-and-bounce animation on a canvas
- 9:16, 1:1 and 16:9 output formats
- EN / TL interface toggle
- Record the animation as a silent WebM clip (`MediaRecorder` + `canvas.captureStream`)

## Run
Open `index.html`. No build step.

## Notes
- Browsers can't capture speech-synthesis audio, so recorded clips are silent. Add a voiceover in a video editor.
- Available voices depend on the user's OS and browser. Filipino voices may be missing.
