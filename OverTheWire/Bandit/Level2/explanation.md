# Bandit Level 2 → Level 3 | Explanation

## 🧠 Core Idea
This level is designed to demonstrate how to work with **filenames that contain spaces**, which can break standard shell command behavior if not handled properly.

---

## 🗂️ Problem
The file containing the password is named `spaces in this filename`. When used unquoted, the shell interprets it as **four separate arguments**, causing commands like `cat` to fail.

---

## 🛠️ Solution Strategy

- If you run:
  ```
  cat spaces in this filename
  ```
  the shell thinks you're trying to `cat` four different files named `spaces`, `in`, `this`, and `filename`.

- Instead, use **quotes** or **escape characters** to ensure the shell treats the whole filename as a single string:

  - Using double quotes:
    ```
    cat "spaces in this filename"
    ```

  - Using backslashes to escape spaces:
    ```
    cat spaces\ in\ this\ filename
    ```

---

## 🧩 Takeaway
- This level teaches the importance of **quoting or escaping special characters** in file and directory names.
- It’s a common hurdle when scripting or navigating real systems and a fundamental concept in Linux shell environments.