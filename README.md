# BMI-Calculator
This project is built using standard web technologies. Below is an explanation of the core logic and terms used in the source code.
1. Document Object Model (DOM)
   The code interacts with the HTML through the DOM. This is the structure of the web page that JavaScript can read and change.document.getElementById(): This is a built-in function used to "find" an HTML element by its unique ID (like wt for weight or ht for height) so the script can either take information from it or update its text..value: This property captures the specific number or text the user typed into an input box.
2. Variables and Constantsconst:
      Short for "constant." We use this to store data that doesn't change once the calculation is done (like your weight or height inputs).let: Used for variables that might change. In this code, we use let message because the text changes depending on whether the result is "Normal" or "Overweight."
3. The BMI FormulaThe core logic relies on the standard health formula for Body Mass Index:$$BMI = \frac{weight (kg)}{height (m)^2}$$Unit Conversion: Since users enter height in centimeters (cm), the code divides the input by 100 to convert it to meters (m) before performing the math.** 2 or heightM * heightM: This represents squaring the height, which is a requirement of the BMI formula.
4. Logic & Formattingif / else if / else:
            These are "Conditional Statements." They act like a filter, checking the calculated BMI against health standards to determine which category the user falls into..toFixed(1): This is a JavaScript method that rounds a number to one decimal place (e.g., changing 22.4567 to 22.5). This makes the result much easier for the user to read.
5. Event Listenersonclick="btn()":
               This is an "Event Handler." It tells the browser, "Wait for the user to click this button, and the moment they do, run the function called btn()."
