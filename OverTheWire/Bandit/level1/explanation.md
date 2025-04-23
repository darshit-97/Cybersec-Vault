# Bandit Level 1 → Level 2 | Explanation

## 🧠 Core Idea
This level is designed to introduce the concept of **files with special names**, particularly those that can be confused with command-line flags.

---

## 🗂️ Problem
The file containing the password is named `-`, which is commonly interpreted by Unix commands like `cat` as shorthand for standard input (stdin).

---

## 🛠️ Solution Strategy

- Normally, you might run:
  ```
  cat -
  ```
  But this would make `cat` wait for input from the terminal instead of reading the file.

- To avoid that, we need to **tell `cat` explicitly to treat `-` as a filename**, not an option. This is done using:
  ```bash
  cat ./-
  ```

  - `./-` means: “in the current directory (`.`), the file named `-`”.
  - This bypasses any confusion with `cat` options and reads the file content correctly.

---

## 🧩 Takeaway
- This level tests your understanding of **command-line parsing**.
- It shows how file names starting with `-` can be problematic and how to work around them using `./`.
