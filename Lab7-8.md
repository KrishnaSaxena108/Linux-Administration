# 🧪 Experiment : 7 - 8

## 📌 Objective

Learn how to:

- Create directories.
- Modify directory permissions using **symbolic** and **octal** methods.
- Set appropriate group and others permissions.
- Change and verify **umask** settings for a specific user.

---

## 📝 Description

In Linux administration, controlling access to directories and files is crucial.  
This experiment covers:

- Creating the `/home/consultants` directory.
- Assigning **write permissions** to the `consultants` group using the **symbolic method**.
- Denying access to others using the **octal method**.
- Changing the default **umask** for a specific user to restrict permissions.
- Verifying the changes.

---

## 🚀 Tasks

### 1️⃣ Create `/home/consultants` Directory

```bash
# Creating Directories With Super User
sudo mkdir /home/consultants
```

### 🖼️ Screenshots

![Screenshot 2025-03-19 184514](https://github.com/user-attachments/assets/3076d421-b4b0-41a2-b7d4-674bd3618e56)

---

### 2️⃣ Add Write Permission to Consultants Group (Symbolic Method)

```bash
# Adding Write Permissions
sudo chmod g+w /home/consultants
```

### 🖼️ Screenshots

![image](https://github.com/user-attachments/assets/99f2bd03-9f79-4df8-be7e-ba118e47ef8d)

---

### 3️⃣ Forbid Others from Accessing /home/consultants (Octal Method)

```bash
# Forbidding Others from Accessing
sudo chmod 770 /home/consultants
```

### 🖼️ Screenshots

![image](https://github.com/user-attachments/assets/8831a2b6-884e-4ce7-bb0b-d2ec74db4702)

---

### 4️⃣ Change Default Umask for operator1 User

1. Open the .bashrc or .bash_profile of user1:
```bash
# Open the .bashsrc file in nano editor
sudo nano /home/user1/.bashrc
```

2. Add this line at the end:
```bash
# For changing the umask value add rhis line in end of the file
umask 007
```

3. Save and exit (`Ctrl + O`, `Enter`, `Ctrl + X`).

### 🖼️ Screenshots

![image](https://github.com/user-attachments/assets/9cce99d1-9253-4c74-80a6-5006b81c711b)

---

### 5️⃣ Confirm the Umask

```bash
# To verify the value of umask
umask
```

### 🖼️ Screenshots

![image](https://github.com/user-attachments/assets/0139f5c2-0d37-4611-9e24-b5b23dd37225)

---

### 🎯 Summary
- Created `/home/consultants` directory.
- Set group write permissions (symbolic method).
- Removed others' access (octal method).
- Changed and verified umask for `user`.
