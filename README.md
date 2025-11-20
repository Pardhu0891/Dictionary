📘 Modern Dictionary

A simple GUI-based dictionary application built entirely in Python using Tkinter, Pillow, and a JSON-based word database. It allows users to search for words, view meanings, and even get suggestions for close matches if the word is spelled incorrectly.

🚀 Features

🔍 Search any word from a large JSON dictionary.

📝 Displays the meaning in a text area with a clean UI.

🎯 Close-match suggestion using difflib.get_close_matches() when the word is mistyped.

🖼️ Attractive GUI built using Tkinter with an image banner.

🪶 Fast and lightweight, no external API calls.

📂 Uses a local JSON file as a dictionary data source.

🛠️ Technologies Used

Python 3

Tkinter (GUI framework)

Pillow (PIL) for image handling

JSON for storing dictionary entries

Difflib for close-match word suggestions

📁 Project Structure
Dictionary/
│
├── Dictionary_code.py        # Main Python application (Tkinter UI + logic)
├── data_dictionary.json      # Dictionary data source (word → meaning)
├── dict.png                  # Banner image displayed in GUI
└── README.md                 # Project documentation

▶️ How to Run the Project
1️⃣ Install Dependencies
pip install pillow

2️⃣ Ensure Required Files Exist

Place the following in the same directory:

Dictionary_code.py

data_dictionary.json

dict.png

3️⃣ Run the Application
python Dictionary_code.py

📸 Screenshots (Optional)

Add screenshots of your GUI here if you want later.

🧠 How It Works
Loading the Dictionary
f = open("data.json")
data_load = json.load(f)

Searching a Word

If the word exists → show exact meaning

If not → find closest match and suggest it

If nothing matches → display nothing (could be improved)

Close-Match Logic
get_close_matches(word, data_load.keys())

📌 Future Improvements (Suggestions)

Add “Word Not Found” message

Add pronunciation

Add multiple meaning support

Add dark mode

Add speech-to-text word search

Convert to .exe using PyInstaller

📄 License

This project is open-source and free to use under the MIT License.
