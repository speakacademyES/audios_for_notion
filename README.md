# Audio Player with Synchronized Transcripts

A single, reusable audio player that displays synchronized transcripts with real-time highlighting. Perfect for embedding in Notion or any website.

## 🎯 How It Works

One player file (`index.html`) + URL parameters = unlimited audio lessons.

## 🚀 Setup (One Time Only)

1. **Upload to GitHub:**
   - `index.html` (your player)
   - Create `audio/` folder → upload your MP3 files
   - Create `transcripts/` folder → upload your VTT files

2. **Enable GitHub Pages:**
   - Go to Settings → Pages
   - Select your branch (main)
   - Save

3. **Your base URL:**
```
   https://yourusername.github.io/repo-name/
```

## 📝 Adding a New Lesson

1. Upload `lesson-name.mp3` to `audio/` folder
2. Upload `lesson-name.vtt` to `transcripts/` folder
3. Use this URL format:
```
https://yourusername.github.io/repo-name/?audio=audio/lesson-name.mp3&vtt=transcripts/lesson-name.vtt&title=Lesson Title
```

## 💡 URL Format
```
https://yourusername.github.io/repo-name/?audio=audio/FILENAME.mp3&vtt=transcripts/FILENAME.vtt&title=YOUR_TITLE
```

**Change only:**
- `FILENAME.mp3` → your audio file
- `FILENAME.vtt` → your transcript file
- `YOUR_TITLE` → lesson title (use `%20` for spaces)

## 📱 Embedding in Notion

1. In Notion, type `/embed`
2. Paste your URL with parameters
3. Done!

## 🔧 File Structure
```
your-repo/
├── index.html
├── audio/
│   ├── lesson1.mp3
│   ├── lesson2.mp3
│   └── lesson3.mp3
└── transcripts/
    ├── lesson1.vtt
    ├── lesson2.vtt
    └── lesson3.vtt
```

## 📖 VTT Format

Create a `.vtt` file with timestamps:
```
WEBVTT

00:00:00.000 --> 00:00:05.000
First line of text.

00:00:05.000 --> 00:00:10.000
Second line of text.
```

## ✨ Examples
```
Lesson 1:
https://yoursite.com/?audio=audio/grammar.mp3&vtt=transcripts/grammar.vtt&title=Grammar Basics

Lesson 2:
https://yoursite.com/?audio=audio/vocabulary.mp3&vtt=transcripts/vocabulary.vtt&title=Essential Vocabulary
```

---

**One player. Infinite lessons. Simple.**