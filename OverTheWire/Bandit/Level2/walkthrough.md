# Bandit Level 2 → Level 3 | Walkthrough

## 🎯 Objective
> The password for the next level is stored in a file called `spaces in this filename` located in the home directory.

- **Hostname**: `bandit.labs.overthewire.org`
- **Port**: `2220`
- **Username**: `bandit2`
- **Password**: `CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`

---

## 🚀 Steps

1. Connect to the server using SSH:

   ```bash
   ssh bandit2@bandit.labs.overthewire.org -p 2220
   ```

2. Once logged in, list the files in the current directory:

   ```bash
   ls
   ```

   You'll see a file named:

   ```
   spaces in this filename
   ```

3. To view the contents of this file, you need to handle the spaces in the filename.

   You can either:
   - Use quotes:

     ```
     cat "spaces in this filename"
     ```

   - Or escape the spaces with backslashes:

     ```
     cat spaces\ in\ this\ filename
     ```

4. This will reveal the password for **Level 3**.

---

## 🧠 Reminder
> These challenges are designed to improve your understanding of the Linux shell. Take a moment to explore and understand why special characters (like spaces) matter in filenames.