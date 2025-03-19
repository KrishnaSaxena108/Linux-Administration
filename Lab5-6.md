# 🧪 Experiment : 5 - 6

## 📌 Objective

Learn how to:

- Edit a file using **Vim** and **Nano** editors.
- Use **shell variables** to reference file names.
- Enter **Visual Mode in Vim**.
- Modify specific content in the file:
  - Remove the last seven characters from the first column on the first line.
  - Preserve only the first four characters of the first column.

---

## 📝 Description

This experiment focuses on basic yet powerful text editing skills using command-line editors:

- **Vim**: A versatile editor with powerful navigation and editing features.
- **Nano**: A beginner-friendly, straightforward editor.

You will also learn how to:

- Use shell variables to manage file names.
- Apply **Visual Mode in Vim** to select and edit content precisely.

---

## 🚀 Tasks

### 1️⃣ Set the Shell Variable

First, set a shell variable to store the filename:

```bash
# Create Shell Variable
lab_file=editing_final_lab.txt
```

To Verify:

```bash
# Print the value of the variable (i.e. editing_final_lab.txt)
echo $lab_file
```

### 🖼️ Screenshot

![Screenshot 2025-03-19 181250](https://github.com/user-attachments/assets/4d2379b0-d88c-4907-955b-de653bf6ff1f)

---

### 2️⃣ Edit Using Vim

Open the file in Vim using the variable:

```bash
# Open the file in vim editor
vim $lab_file
```

🔽 Steps Inside Vim:

- Press `Esc` to ensure you're in **Normal Mode**.
- Move to the **first line** (use `gg` shortcut).
- Move the cursor to the **first column**.
- Press `v` to enter **Visual Mode**.
- Use arrow keys or `l` (right move) to select characters.
- **Delete last 7 characters** from the first column (use `x` to delete selected).
- Ensure only the **first 4 characters** remain.
- Save & exit:
```bash
# For exiting vim editor type it in the editor and hit enter
:wq
```

### 🖼️ Screenshot

![Screenshot 2025-03-19 182728](https://github.com/user-attachments/assets/3d82acdb-5151-438f-92ba-6821ff7fcdb9)

---

### 3️⃣ Edit Using Nano

Open the file in Nano:

```bash
# Open the file in nano editor
nano $lab_file
```

🔽 Steps Inside Nano:
- Use arrow keys to move to the **first line**.
- Delete the unwanted characters manually:
- Remove the last 7 characters from the first column.
- Keep only the first 4 characters.
- Save:
Press `Ctrl + O`, hit `Enter`.
- Exit:
Press `Ctrl + X`.

### 🖼️ Screenshot

![Screenshot 2025-03-19 183522](https://github.com/user-attachments/assets/6826745e-6e4b-4bc6-8409-68e46d4f7612)

---

### 🎯 Summary
- Set shell variable to hold file name.
- Edited file using **Vim** and **Nano**.
- Practiced **Visual Mode in Vim** for precise editing.
- Modified specific content as required.
