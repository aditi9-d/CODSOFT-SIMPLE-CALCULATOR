# Simple GUI Calculator

A clean, functional, and user-friendly calculator built with Python's built-in Tkinter library. This project provides a graphical user interface for performing basic arithmetic operations like addition, subtraction, multiplication, and division.

It's a great example of how to create a simple desktop application using standard Python libraries, perfect for beginners learning GUI development.

---

## ► Features

- **Standard Arithmetic Operations:** Perform addition (`+`), subtraction (`-`), multiplication (`*`), and division (`/`).
- **User-Friendly Interface:** A classic calculator layout with a clear display and responsive buttons.
- **Error Handling:** Gracefully handles invalid expressions (e.g., `5 * `) and division by zero, displaying an "Error" message.
- **Clear Functionality:** A 'C' button to easily clear the current expression and start fresh.
- **Responsive Design:** A fixed-size window that maintains its layout and appearance.

---

## ► How to Run

This calculator is built using Python and its standard Tkinter library, so you don't need to install any external packages.

**Prerequisites:**
- Python 3 installed on your system.

**Instructions:**

1.  **Clone the repository or download the source code:**
    ```bash
    git clone [https://github.com/aditi9-d/simple-calculator.git](https://github.com/your-username/simple-calculator.git)
    cd simple-calculator
    ```

2.  **Run the Python script:**
    ```bash
    python calculator_script.py
    ```
    *(Assuming you've saved the code from the notebook as `calculator_script.py`)*

The calculator window will appear, and you can start performing calculations.

---

## ► Code Overview

The application is built within a single Python script and is structured as follows:

### 1. Core Functions

-   `on_button_click(char)`: Appends the character of the pressed button (number or operator) to the current expression string and updates the display.
-   `calculate_result()`: Evaluates the expression string using Python's `eval()` function when the `=` button is pressed. It handles potential `SyntaxError` or `ZeroDivisionError` exceptions.
-   `clear_display()`: Resets the expression string and clears the calculator's display when the 'C' button is pressed.

### 2. GUI Setup (Tkinter)

-   **Main Window:** A `tk.Tk()` object is created to serve as the main application window. Its title, size, and background color are configured.
-   **Display Screen:** A `tk.Entry` widget is used for the calculator's display. It's right-aligned and styled to look like a typical calculator screen. A `tk.StringVar()` is used to link the display widget with the `expression` variable.
-   **Button Layout:** The calculator buttons are created in a loop. They are placed in a `tk.Frame` using the `.grid()` layout manager to achieve the classic calculator layout.
-   **Button Styling:** Buttons are styled differently based on their function (numbers, operators, or the clear button) for better visual distinction.
-   **Event Loop:** `window.mainloop()` starts the Tkinter event loop, which listens for user actions like button clicks and keeps the application running.

---

## ► Dependencies

-   **Python 3**
-   **Tkinter:** This is part of Python's standard library and usually comes pre-installed with Python. No separate installation is needed.

