﻿# JavaFxCalculator
How the Code Works:
Model (Calculator Class):

The Calculator class is responsible for all the math operations. It stores the numbers (operands) and the operator (like +, -, *, or /). It also checks if any errors occur (for example, division by zero).
When the user clicks an operator or the equals button, the Calculator performs the calculation and returns the result. There are methods to set the numbers and operator, perform the calculation, and reset everything when needed.
View (FXML Layout):

The layout of the calculator (the buttons, text field, etc.) is defined in an FXML file. There’s a text field to show the input and results, and buttons for digits (0-9), operators (+, -, *, /), the equals sign (=), and a clear button (C).
This layout is what the user sees and interacts with on the screen.
Controller (CalculatorController Class):

The CalculatorController class connects the buttons and text field to the Calculator logic. It responds when buttons are pressed:
If a number button is pressed, it shows that number in the text field.
If an operator is pressed, it saves the first number (operand1) and waits for the next number (operand2).
When the equals button is pressed, it calculates the result based on the two numbers and the operator.
If the clear button is pressed, it resets everything so the user can start a new calculation.
The controller makes sure that any errors (like dividing by zero) are handled and displays an error message if needed.
Application Entry Point (Main Class):

The Main class is where the JavaFX application starts. It loads the FXML file that defines the layout and opens the calculator window.
Example:
When the user clicks the number 5, it is displayed in the text field.
If the user then clicks the + button, the calculator saves 5 as the first number and waits for the second number.
When the user clicks 3 and then =, the calculator adds 5 and 3 together and shows the result (8) in the text field.
If the user presses the C button, it clears everything and lets them start a new calculation.
