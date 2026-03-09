# 🐝 BeeLingual — Vocabulary Building App

## Description

BeeLingual is a desktop flashcard application built with Python that helps users learn vocabulary in 6 foreign languages — French, German, Mandarin, Portugese, Russian, and Spanish.

With traditional learning methods, it is difficult to learn thousands of new words. People who want to learn a foreign language find it hard to understand and remember so many words. BeeLingual solves this by providing a digital platform that makes the learning process much easier and more engaging.

The app uses flashcards to promote active recall — a process where students actively stimulate their memory to create lasting connections to the material. Each flashcard displays a foreign word on the front, then flips after 3 seconds to reveal the English translation. Audio pronunciation is played automatically using Google Text-to-Speech, making it easier to learn correct pronunciation in a fun way.

---

## 🌍 Supported Languages

| Language | Launcher |
|----------|----------|
| 🇫🇷 French | `French.py` |
| 🇩🇪 German | `German.py` |
| 🇨🇳 Mandarin | `Mandarin.py` |
| 🇵🇹 Portugese | `Portugese.py` |
| 🇷🇺 Russian | `Russian.py` |
| 🇪🇸 Spanish | `Spanish.py` |

---

## ✨ Features

- 🃏 **Flashcard UI** — Shows the foreign word on the front, flips to English after 3 seconds
- 🔊 **Audio Pronunciation** — Speaks each word aloud using Google TTS (requires internet)
- ✅ **Progress Tracking** — Words you mark as known are removed and progress is saved automatically
- 🔁 **Smart Review** — On restart, only shows words you haven't learned yet
- 🏆 **Completion Alert** — Congratulates you when all words are reviewed

---

## 🚀 How to Run

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
├── French.py
├── German.py
├── Mandarin.py
├── Portugese.py
├── Russian.py
├── Spanish.py
│
├── data/
│   ├── french_words.csv
│   ├── german_words.csv
│   ├── mandarin_words.csv
│   ├── portugese_words.csv
│   ├── russian_words.csv
│   ├── spanish_words.csv
│   └── words_to_learn.csv      ← Auto-generated (saves your progress)
│
└── images/
    ├── card_front.png
    ├── card_back.png
    ├── right.png
    └── wrong.png
```

---

## 🎮 How to Use

1. Run any language script (e.g. `python French.py`)
2. A flashcard appears showing a **foreign word** — try to recall the English meaning
3. After **3 seconds**, the card flips to show the **English translation** and plays pronunciation
4. Click ✅ **Right** if you knew it — the word is removed from your list
5. Click ❌ **Wrong** if you didn't — the word stays in rotation
6. Your progress is saved automatically — close and resume anytime

---

## 🛠️ Built With

- **Python 3.10** — Core language
- **Tkinter** — Desktop GUI
- **gTTS** (Google Text-to-Speech) — Audio pronunciation
- **Pandas** — Word data management
- **Playsound** — Audio playback
- **VS Code** — Editor
- **Google Sheets** — Word dataset preparation (with `GOOGLETRANSLATE` formula)

---

## ⚠️ Limitations

- Features only frequently used words (no grammar or sentence construction)
- Works on Windows only
- Requires an active internet connection
- Words are not categorized (e.g. by topic like Animals, Food, etc.)

---

## 🔮 Future Enhancements

- Category-wise word selection (Animals, Fruits, Family, etc.)
- Sentence construction and grammar support
- Images for better word interpretation
- Customizable audio repetition
- Offline mode

---

## 👥 Team

| Name | Roll No | Contribution |
|------|---------|-------------|
| **Anjor Sunil Patil** | 52 | Audio integration using gTTS & playsound |
| **Gauri Sanjeev Wagh** | 53 | GUI design using Tkinter |
| **Shriya Sushant Parange** | 16 | Combined GUI + audio, converted to executable |

**Guide:** Mrs. Kirti Garud

---

## 📚 References

- https://docs.python.org/3/library/tkinter.html
- https://gtts.readthedocs.io/en/latest/
- https://www.geeksforgeeks.org/play-sound-in-python/
- https://www.geeksforgeeks.org/convert-text-speech-python/
- https://www.geeksforgeeks.org/introduction-to-pandas-in-python/
