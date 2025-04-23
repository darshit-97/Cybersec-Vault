# Bandit Level 0 → Level 1

## 🧠 Goal
Learn how to connect to a remote machine using SSH.

## 🎯 Level Goal
> The password for the next level is stored in a file called `readme` located in the home directory. Use SSH to log into the server using the given credentials.
  
- **Hostname**: `bandit.labs.overthewire.org`  
- **Port**: `2220`
- **Username**: `bandit0`
- **Password**: `bandit0`

## 💻 Commands Used

```
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
- `ssh`: Secure Shell, used to connect to remote machines securely.
- `bandit0@...`: Username followed by host (the remote server).
- `-p 2220`: Specifies the port (Bandit runs on port 2220, not the default 22).

```
ls
```
- `ls`: Lists files and directories in the current location.

```
cat readme
```
- `cat`: Concatenates and prints the content of a file—in this case, the password.

## 🔐 Password for Level 1
```
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```

## 📝 Notes
- This level introduces the **SSH** protocol, foundational for all remote server interactions.
- The file was easily visible using `ls`, and I used `cat` to read its contents.
- Linux is case-sensitive, so be exact with filenames.