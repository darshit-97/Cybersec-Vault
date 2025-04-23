### 📘 `commands.md`

```
# Bandit Level 1 → Level 2 | Commands Used

## 🔐 SSH into the Level
```
ssh bandit1@bandit.labs.overthewire.org -p 2220
```
- `ssh`: Command to securely connect to the remote server.
- `bandit1@...`: Username and hostname of the Bandit server.
- `-p 2220`: Specifies the non-default port used by Bandit.

---

## 📁 List Files
```
ls
```
- Lists the files in the current directory.
- Reveals a file named `-`.

---

## 📖 Read the File Named `-`
```
cat ./-
```
- `cat`: Reads the contents of files.
- `./-`: Tells the system to read a file named `-` in the current directory, avoiding confusion with command-line flags.

---

## 📝 Notes
- If you had used `cat -`, it would wait for user input instead of reading the file.
- The `./` prefix is essential when handling files with names that might be interpreted as options.
```