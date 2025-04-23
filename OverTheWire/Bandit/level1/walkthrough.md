# Bandit Level 1 → Level 2 | Walkthrough

## 🎯 Objective
The password for the next level is stored in a file called - located in the home directory

---

## 🚀 Steps

1. **Login to the server**
   ```
   ssh bandit1@bandit.labs.overthewire.org -p 2220
   ```

2. **List the files**
   ```
   ls
   ```
   - Output: `-`

3. **Display the contents of `-`**
   ```
   cat ./-
   ```
   - This reveals the password for Level 2.

---

## 🔐 Output (Password for Level 2)

```
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```
