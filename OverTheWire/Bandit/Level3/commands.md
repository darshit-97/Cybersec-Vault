# Bandit Level 3 → Level 4 | Commands Used

## 🔐 SSH into the Level
```
ssh bandit3@bandit.labs.overthewire.org -p 2220
```
- Connects to the Bandit server using the credentials for Level 3.

---

## 📂 Navigate into the `inhere` Directory
```
cd inhere
```
- `cd`: Changes the current working directory.
- `inhere`: The folder that contains the hidden file.

---

## 👻 Show Hidden Files
```
ls -a
```
- `ls`: Lists files and directories.
- `-a`: Reveals all files, including hidden ones (those starting with a dot `.`).

---

## 📖 Read the Hidden File
```
cat .hiddenfilename
```
- `cat`: Reads the content of files.
- `.` at the beginning of the filename indicates it’s hidden.
- If the filename has spaces or symbols, use quotes:
  ```
  cat "...Hiding-From-You"
  ```

---

## 📝 Notes
- Hidden files are common in Linux and are often used to store configuration or secret data.
- `ls -a` is essential when files aren’t visible with a standard `ls`.