### **Bandit Level 3 → Level 4 | Walkthrough**

## 🎯 Objective
> The password for the next level is stored in a hidden file in the `inhere` directory.

- **Hostname**: `bandit.labs.overthewire.org`
- **Port**: `2220`
- **Username**: `bandit3`
- **Password**: `UoMYtrfrBFHy7W9k7jYpR5kJt9SOmJpG`

---

## 🚀 Steps

1. Connect to the server using SSH:

   ```
   ssh bandit3@bandit.labs.overthewire.org -p 2220
   ```

2. Once logged in, navigate to the `inhere` directory:

   ```
   cd inhere
   ```

3. List all files, including hidden ones:

   ```
   ls -a
   ```

   - **Why `-a` flag?**  
     This flag lists **all** files, including hidden ones (those that start with `.`).

4. Find the hidden file, which might look something like `.hidden` or `...Hiding-From-You`.

5. Use `cat` to read the file:

   ```
   cat .hidden
   ```

   Or if you found a file with special characters (e.g., spaces):

   ```
   cat "...Hiding-From-You"
   ```

6. The content of the file will reveal the password for **Level 4**.