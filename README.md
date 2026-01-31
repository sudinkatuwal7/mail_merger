# 📬 Mail Merge Project

## 🌟 Overview

The **Mail Merge Project** is a simple Python program that automates the process of creating **personalized letters** for multiple recipients. Instead of manually editing a template letter for each person, this program reads a list of names and generates a separate letter for each individual with their name inserted at the designated placeholder. ✨

---

## 📂 File Structure
```bash
Mail_Merge_Project/
│
├── Input/
│ ├── Letter/
│ │ └── starting_letter.txt # 📝 Template letter with placeholder for names
│ │
│ └── Names/
│ └── invited_names.txt # 🧑‍🤝‍🧑 List of recipient names
│
├── Output/
│ └── ReadyToSend/ # ✉️ Folder where personalized letters are saved
│
├── main.py # 🐍 Python script for the mail merge
└── README.md # 📖 Project description and instructions
```

---


---

## 🔧 How It Works

1. The program reads a **template letter** from `input/Letter/starting_letter.txt`.  
   - The template contains a placeholder `[name]` where each recipient's name will be inserted. ✍️

2. It reads a list of **recipient names** from `input/Names/invited_names.txt`. 📄

3. For each name in the list:
   - Strips any extra spaces or newline characters. 🧹  
   - Replaces the placeholder `[name]` in the template with the recipient's name. 🖊️  
   - Saves the personalized letter to `output/ReadyToSend/` with a filename like `letter_for_<Name>.txt`. 💌

---

## 📖 Example

**Template (`starting_letter.txt`):**

Dear [name],

Hey, how have you been doing? It's been a while since we had a cup of coffee together. Life is full of
unpredictable outcomes pretty much like a TRNGs. We can never predict where we will be in the recent years.
Leave that discussion to that, you are such a special to me , so I want to give you a treat for such a beautiful 
surprise. Make sure to be at my house at sharp 5 pm or if possible even before on Friday night.

Hope you can make it!

Sudin

---

**Personalized Letter (`letter_for_Suyog.txt`):**

Dear Suyog,

Hey, how have you been doing? It's been a while since we had a cup of coffee together. Life is full of
unpredictable outcomes pretty much like a TRNGs. We can never predict where we will be in the recent years.
Leave that discussion to that, you are such a special to me , so I want to give you a treat for such a beautiful 
surprise. Make sure to be at my house at sharp 5 pm or if possible even before on Friday night.

Hope you can make it!

Sudin

---


## 🚀 How to Run

### Make sure you have **Python 3.x** installed 🐍
   
### Navigate to the project directory:  
   ```bash
   cd Mail_Merge_Project
   ```
### Run the script:
```
python main.py
```
**Check the Output/ReadyToSend/ folder for your personalized letters**

---

## ⚠️ Notes

The program overwrites any existing files in output/ReadyToSend/ with the same names. 🔄

Ensure that the folder Output/ReadyToSend/ exists before running the script, or modify `main.py` to create it automatically:
```bash
import os

os.makedirs("Output/ReadyToSend", exist_ok=True)
```
"At the top before the code."

`You can customize the template letter and the list of names as needed. ✨`
