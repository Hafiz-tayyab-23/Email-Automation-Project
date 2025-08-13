# 📧 Email Extractor from Text Files

**A lightweight Python automation tool** that scans `.txt` files, extracts all email addresses, removes duplicates, and saves a clean, sorted list — in seconds. Perfect for **newsletters, mailing lists, and bulk contact cleanup**.

---

## 🔍 Overview

This Python script automates a small but common repetitive task — extracting all email addresses from a `.txt` file and saving them into a separate file.
It uses Python’s built-in **`re`** (regular expressions) module for pattern matching and **file handling** for reading and writing data.

---

## ✨ Features

* 📂 Scans any `.txt` file for valid-looking email addresses.
* 🧹 Automatically removes duplicates.
* 📑 Sorts emails alphabetically before saving.
* 💾 Saves the clean list of emails into a specified output file.
* ⚡ Simple & lightweight — **no external libraries required**.

---

## ⚙ How It Works

1. **Prompts the user** for:

   * The input file path (the `.txt` file to scan).
   * The output file name (where extracted emails will be stored).
2. Reads the input file content.
3. Uses a **regular expression** to find all email addresses in the text.
4. Removes duplicates and sorts them alphabetically.
5. Writes the final list to the output file.
6. Displays the **number of unique email addresses** found.

---

## 💻 Example Usage

```bash
$ python email_extractor.py
Enter the path to the .txt file to scan for emails: source_file.txt
Enter the filename to save found email addresses: destination_file.txt
Found 312 unique email addresses. Saved to extracted_emails.txt.
```

---

## 🧠 Regex Pattern Used

```python
r"[\w\.-]+@[\w\.-]+"
```

* `[\w\.-]+` → Matches one or more letters, digits, underscores, dots, or hyphens.
* `@` → Matches the literal "@" symbol.
* `[\w\.-]+` → Matches the domain part of the email.

---

## 📋 Requirements

* Python **3.x**
* No external dependencies

---

## 📂 File Structure

```
.
├── email_extractor.py         # Main script
├── source_file.txt            # Example input file
├── destination_file.txt       # Example output file
└── README.md                  # Documentation
```

---

## 📌 About

Built to **save hours of manual data cleaning** for large text datasets. Ideal for quick, offline email extraction without installing heavy software or libraries.

---
