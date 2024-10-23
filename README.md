# Quizler App

**Quizler** is a Python-based quiz application built using the `Tkinter` library for the graphical user interface. It presents true/false quiz questions and keeps track of the user's score. The app dynamically loads quiz questions and displays them one by one, allowing users to answer by clicking the "True" or "False" buttons.

## Features
- GUI built with Tkinter
- True/False quiz questions
- Displays the current score as the quiz progresses
- Provides feedback on whether the answer was correct or not
- Gracefully handles the end of the quiz by disabling the answer buttons and showing a completion message

## Requirements

Before running the project, make sure you have Python installed on your machine. You will also need the following libraries:

- `tkinter`: Python's standard GUI library
- `html`: Standard library to handle HTML encoding (already available in Python)

## Setup

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/your-username/quizler-app.git
    ```

2. Navigate to the project directory:

    ```bash
    cd quizler-app
    ```

3. Install dependencies (if needed):

    - For `tkinter`: Usually comes with Python, but if not installed, you can install it using the following command for Linux:
      ```bash
      sudo apt-get install python3-tk
      ```

    - For Windows, `tkinter` should be bundled with your Python installation.

4. Ensure the required directories and files exist:
    - **Images**: Ensure that there is a directory named `images` containing the following:
        - `true.png`: Image for the true button
        - `false.png`: Image for the false button

5. Run the application:

    ```bash
    python main.py
    ```

## Project Structure

```bash
quizler-app/
│
├── images/
│   ├── true.png          # Image for the True button
│   └── false.png         # Image for the False button
│
├── data.py               # Contains question data (replace with API if needed)
├── question_model.py     # Defines the Question class
├── quiz_brain.py         # Handles quiz logic (checking answers, loading next question)
├── ui.py                 # Handles the user interface with Tkinter
└── main.py               # Runs the application
