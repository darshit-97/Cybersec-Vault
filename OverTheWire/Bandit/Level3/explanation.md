### **Bandit Level 3 → Level 4 | Explanation**

## 🧠 Core Idea
This level introduces **hidden files**—files that are not visible with a standard `ls` command because their names begin with a dot (`.`).

---

## 🗂️ Problem
You're told the password is stored in a **hidden file** inside the `inhere` directory. But when you run a normal `ls`, nothing shows up.

---

## 🛠️ Solution Strategy

- First, enter the `inhere` directory using:
  ```
  cd inhere
  ```

- Use the `ls` command with the `-a` (or `--all`) flag:
  ```
  ls -a
  ```
  - This reveals all files, including hidden ones (those starting with `.`).

- Once you identify the hidden file, use `cat` to read its contents:
  ```
  cat .<filename>
  ```

  - If the filename includes special characters (like spaces or symbols), wrap it in quotes:
    ```
    cat "...Hiding-From-You"
    ```

---

## 🧩 Takeaway
- This level teaches the importance of **hidden files** in Unix-like systems.
- It also builds your understanding of how to **navigate the filesystem** more precisely and reveals another layer of how Linux treats filenames starting with `.`.