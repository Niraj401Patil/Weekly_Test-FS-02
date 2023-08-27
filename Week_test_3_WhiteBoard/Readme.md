 
# White Board

A basic web-based paint application built using HTML, CSS, and JavaScript. This app allows users to draw on a canvas, delete the drawing, and undo the last drawn stroke.



## Features

- Drawing on canvas using the mouse.
- Deleting the entire drawing.
- Undoing the last drawn stroke.

## Demo

Check out the live demo: [Simple White Board App](https://niraj401patil.github.io/FS-02-M6/Week_Test_3_WhitBoard/)

## Getting Started

1. Clone this repository to your local machine:

2. Open the `index.html` file in a web browser to launch the paint app.



### HTML and CSS

The paint app consists of a canvas element where users can draw. The canvas is styled using CSS to provide a border.

### JavaScript Functionality

1. **Drawing**: When the user presses the mouse button (`mousedown`) on the canvas, the `startPosition` function is triggered. This sets the `painting` flag to `true` and records the initial position. The `mousemove` event triggers the `draw` function, which draws lines on the canvas as the mouse moves. When the user releases the mouse button (`mouseup`), the `endPosition` function is called, and the drawn stroke is saved as an `ImageData` object in the `strokes` array.

2. **Delete**: The "Delete" button clears the entire canvas by using the `clearRect` method. It also clears the `strokes` array to remove any saved strokes.

3. **Undo**: The "Undo" button uses the `putImageData` method to redraw the previously saved strokes when clicked. The `undoButton` event listener removes the last stroke from the `strokes` array and calls the `redraw` function, which iterates through the `strokes` array and redraws the saved strokes.

## Conclusion :

Thank you for checking out this simple paint app! I hope you find it helpful as a starting point for creating your own drawing applications or learning about HTML5 canvas and basic JavaScript interactivity. If you have any questions or ideas for improvements, please don't hesitate to reach out.

