# Contact Form with JavaScript Validation

This repository contains the solution for **Task 6** of the Web Development Internship.

---

## Task Objective

The goal of this task was to build an HTML **Contact Form** that includes **client-side validation** using JavaScript. The form collects a user's **Name**, **Email**, and **Message**, and ensures that:

* All fields are filled out.
* The email address is in a valid format.
* Proper user feedback is shown for both errors and successful submission.

---

## Project Structure

```
├── index.html      # Contains the form's HTML structure
├── style.css       # Provides styling for a clean and responsive UI
└── script.js       # Handles form validation and user feedback
```

---

## How the Solution Works

### 1. HTML Structure

* The form is built using semantic elements like `<form>`, `<label>`, `<input>`, and `<textarea>`.
* Each input field has an associated `<div>` to display error or success messages dynamically.

### 2. CSS Styling

* The form is styled for simplicity and readability.
* Uses consistent spacing, borders, and colors.
* Includes styles for:

  * Error messages (red text)
  * Success messages (green text)
  * Responsive layout for different screen sizes.

### 3. JavaScript Validation

* The script waits for the `DOMContentLoaded` event before running.
* It listens to the form’s `submit` event and prevents default submission using `event.preventDefault()`.
* Validation steps:

  * Checks that **Name** and **Message** are not empty.
  * Validates **Email** using a regular expression (Regex).
* Provides **dynamic feedback**:

  * Displays error messages if validation fails.
  * Shows a “Success!” message and clears the form with `contactForm.reset()` if validation passes.

---

## Key Concepts Implemented

* **Form Elements** (`<form>`, `<input>`, `<textarea>`)
* **Event Handling** (`submit` event listener)
* **DOM Manipulation** (`getElementById`, `.textContent`, `.classList`)
* **Client-Side Validation** (JavaScript)
* **Regular Expressions (Regex)** for validating email format

---

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/SahanaLachyan08/task-6.git
   ```
2. Open the project folder:

   ```bash
   cd task-6
   ```
3. Open `index.html` in your web browser.
