# 🐝 BeeLingual — Vocabulary Building App

A flashcard-based desktop vocabulary learning app that helps you learn words in **6 languages** with pronunciation audio powered by Google Text-to-Speech.

---

## 🌍 Supported Languages

| Language | Script | Launcher |
|----------|--------|----------|
| 🇫🇷 French | Latin | `French.exe` |
| 🇩🇪 German | Latin | `German.exe` |
| 🇨🇳 Mandarin | Chinese | `Mandarin.exe` |
| 🇵🇹 Portugese | Latin | `Portugese.exe` |
| 🇷🇺 Russian | Cyrillic | `Russian.exe` |
| 🇪🇸 Spanish | Latin | `Spanish.exe` |

---

## ✨ Features

- 🃏 **Flashcard UI** — Shows the foreign word on the front, flips to English after 3 seconds
- 🔊 **Audio Pronunciation** — Speaks each word aloud using Google TTS (requires internet)
- ✅ **Progress Tracking** — Words you mark as known are removed and your progress is saved
- 🎯 **Smart Review** — On restart, only shows words you haven't learned yet
- 🏆 **Completion Alert** — Congratulates you when all words are reviewed

---

## 🚀 How to Run

### Option 1 — Run the `.exe` (Windows, no setup needed)

1. Open the project folder
2. Double-click `index.html` to open the language selector
3. Click any language to launch that app

> **Note:** The `.exe` files require an active internet connection for audio playback.

### Option 2 — Run from Python source

**Requirements:**
- Python 3.10+
- Internet connection (for gTTS audio)

**Install dependencies:**
```bash
pip install gtts playsound pandas
```

**Run a specific language:**
```bash
python French.py
python German.py
python Mandarin.py
# etc.
```

---

## 📁 Project Structure

```
BeeLingual/
│
├── index.html              ← Language selector page
├── img1.jpeg               ← Background image
│
├── French.py / French.exe
├── German.py / German.exe
├── Mandarin.py / Mandarin.exe
├── Portugese.py / Portugese.exe
├── Russian.py / Russian.exe
├── Spanish.py / Spanish.exe
│
├── data/
│   ├── french_words.csv        ← Word dataset
│   ├── german_words.csv
│   ├── mandarin_words.csv
│   ├── portugese_words.csv
│   ├── russian_words.csv
│   ├── spanish_words.csv
│   └── words_to_learn.csv      ← Auto-generated (your progress)
│
└── images/
    ├── card_front.png
    ├── card_back.png
    ├── right.png
    └── wrong.png
```

---

## 🎮 How to Use

1. Launch any language app
2. A flashcard appears showing a **foreign word** — try to recall the English meaning
3. After **3 seconds**, the card flips to show the **English translation** and plays pronunciation
4. Click ✅ **Right** if you knew it — the word is removed from your list
5. Click ❌ **Wrong** if you didn't — the word stays in rotation
6. Your remaining words are saved automatically — you can close and resume anytime

---

## 🛠️ Built With

- **Python 3.10** — Core language
- **Tkinter** — Desktop GUI
- **gTTS** (Google Text-to-Speech) — Audio pronunciation
- **pandas** — Word data management
- **playsound** — Audio playback
- **PyInstaller** — Packaging to `.exe`

---

## 👥 Team

| Name | Role |
|------|------|
| **Anjor Patil** | Developer |
| **Gauri Wagh** | Developer |
| **Shriya Parange** | Developer |

---

## 📝 Notes

- The `data/words_to_learn.csv` file is created automatically to track your progress. Delete it to start over.
- The `.exe` files were built with PyInstaller and tested on Windows 10/11.
- Audio requires an active internet connection (uses Google's TTS servers).
