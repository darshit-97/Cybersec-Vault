# Bandit Level 2 → Level 3 | Commands Used

## 🔐 SSH into the Level
```
ssh bandit2@bandit.labs.overthewire.org -p 2220
```
- `ssh`: Command to securely connect to the remote server.
- `bandit2@...`: Username and hostname of the Bandit server.
- `-p 2220`: Specifies the non-default port used by Bandit.

---

## 📁 List Files
```
ls
```
- Lists the files in the current directory.
- Reveals a file named `spaces in this filename`.

---

## 📖 Read the File Named `spaces in this filename`
```
cat "spaces in this filename"
```
- `cat`: Command used to display the contents of a file.
- `"spaces in this filename"`: The filename containing spaces needs to be wrapped in quotes to prevent the shell from splitting it into separate arguments.

OR 

```
cat spaces\ in\ this\ filename
```
- Alternatively, backslashes (`\`) can be used to escape spaces in the filename.

---

## 📝 Notes
- The file name `spaces in this filename` contains spaces, so you need to either escape the spaces with backslashes or wrap the whole filename in quotes.
- Quoting or escaping filenames with special characters is a crucial part of shell navigation.