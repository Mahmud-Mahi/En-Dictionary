# **Intelligent Offline & Online Dictionary | Smart Word Lookup & Pronunciation**  

A powerful, user-friendly **offline & online dictionary** with an interactive graphical interface. It provides definitions, examples, synonyms, and antonyms for words using both **offline data** and an **online API**.

Additionally, the project includes a **standalone dictionary app** built using PyInstaller, allowing users to use the dictionary without running Python scripts.

## **Features**  

✔ **Offline & Online Search** – Retrieves word details from a local JSON database and an online API if not found offline.  
✔ **Intelligent Word Matching** – Uses Levenshtein distance to suggest similar words if the search term is incorrect.  
✔ **GUI-Based Search** – Built using **Tkinter**, offering an easy-to-use graphical interface.  
✔ **Word Management** – Allows users to **add, edit, and overwrite** words in the offline dictionary.  
✔ **Speech Feature** – Pronounces words using the `espeak-ng` package.  
✔ **Dictionary App** – A compiled **standalone app** built with **PyInstaller**, eliminating the need for Python installation.

---

## **Installation Guide**  

### **For Running as a Python Script**

#### **Linux & macOS**
```sh
sudo apt install espeak-ng   # Install speech package
git clone https://github.com/Mahmud-Mahi/En-dictionary.git  
cd En-dictionary  
pip install -r requirements.txt  
python En-dictionary.py  
```

#### **Windows**
1. Install [Python](https://www.python.org/downloads/) (if not already installed).  
2. Install `espeak-ng` for pronunciation.  
3. Clone the repository and run:
```sh
pip install -r requirements.txt  
python En-dictionary.py  
```

---

### **For Using the Standalone Dictionary App**

#### **For Windows**
1. Open Command Prompt in "En-dictionary" directory.
2. Run:
```sh
pyinstaller --onefile --windowed En-dictionary.py
```
3. The .exe file will be in the "dist" folder in the same directory.
4. Move the "dict" folder to your home directory.
5. Run:
```sh
mv dict ~
```
6. Double-click the .exe file to run the dictionary.

#### **For Linux**
1. Open terminal in "En-dictionary" directory.  
2. Give execution permission:
```sh
chmod +x En-dictionary
```
3. Move the "dict" folder to your home directory.
4. Run:
```sh
mv dict ~
```
5. Open the app:
```sh
./En-dictionary
```

#### **For macOS **
1. Open the terminal & navigate to your project directory.  
2. Run:
```sh
pyinstaller --onefile --windowed En-dictionary.py
```
3. The .app file will be in the "dist" folder in the same directory.
4. Move the "dict" folder to your home directory.
5. Run:
```sh
mv dict ~
```
6. Double-click the .app file to run the dictionary.

___

## **How It Works**  

1. **Searching for a Word:**  
   - Type a word in the search box and press **Enter** or click **Search**.  
   - If the word is found in the offline dictionary, its details will be displayed.  
   - If the word isn’t found, the application will try fetching it from the online API.  

2. **Word Suggestions:**  
   - If a word is misspelled, the program suggests a close match.  
   - You can accept the suggestion or manually add a new word.  

3. **Adding a Word:**  
   - If a word is not found, you can choose to add it to the offline dictionary.  
   - You’ll be prompted to enter a definition, examples, synonyms, and antonyms.  

4. **Editing a Word:**  
   - If a word exists in the dictionary, you can overwrite its details by clicking **Edit**.  

5. **Deleting an Entry (Manually):**  
   - Open `offline_dictionary.json` and remove the desired entry.  

6. **Pronunciation Feature:**  
   - Click **Pronounce** to hear the word spoken using `espeak-ng`.  

---

## **Offline Dictionary File**  
The offline dictionary is stored in:  
```
~/dict/offline_dictionary.json
```
This file is automatically updated whenever a word is added or edited.

---

## **Future Improvements**  
🔹 Add support for more languages.  
🔹 Improve pronunciation with additional voice options.  
🔹 Implement a database for better performance.  

---

## **License**  
This project is open-source and licensed under the **MIT License**.  

---

## **Contributions & Issues**  
Feel free to contribute by submitting pull requests. If you encounter any issues, open a ticket in the GitHub **Issues** section.
