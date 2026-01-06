Here's your updated README file that reflects the current structure and features:

```markdown
# Audio Player with Synchronized Transcripts

A single, reusable audio player that displays synchronized transcripts with real-time highlighting. Perfect for embedding in Notion or any website. Includes optional header images for a more polished look.

## 🎯 How It Works

One player file (`index.html`) + URL parameters = unlimited audio lessons with beautiful headers.

## 🚀 Setup (One Time Only)

1. **Upload to GitHub:**
   - `index.html` (your player)
   - Create `audio/` folder → upload your MP3 files
   - Create `transcripts/` folder → upload your VTT files
   - Create `images/` folder → upload header images (optional)

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
3. (Optional) Upload `lesson-name.jpg` to `images/` folder
4. Use this URL format:
```
https://yourusername.github.io/repo-name/?audio=audio/lesson-name.mp3&vtt=transcripts/lesson-name.vtt&title=Lesson%20Title&image=images/lesson-name.jpg
```

## 💡 URL Format

### With Header Image (Recommended):
```
https://yourusername.github.io/repo-name/?audio=audio/FILENAME.mp3&vtt=transcripts/FILENAME.vtt&title=YOUR_TITLE&image=images/FILENAME.jpg
```

### Without Header Image:
```
https://yourusername.github.io/repo-name/?audio=audio/FILENAME.mp3&vtt=transcripts/FILENAME.vtt&title=YOUR_TITLE
```

**URL Parameters:**
- `audio` = Path to MP3 file (required)
- `vtt` = Path to VTT transcript (required)
- `title` = Lesson title (required, use `%20` for spaces)
- `image` = Path to header image (optional)

## 📱 Embedding in Notion

1. In Notion, type `/embed`
2. Paste your complete URL with parameters
3. Adjust embed height if needed
4. Done!

## 🔧 File Structure
```
your-repo/
├── index.html
├── audio/
│   ├── Compare_Adjectives.mp3
│   ├── lesson2.mp3
│   └── lesson3.mp3
├── transcripts/
│   ├── Compare_Adjectives.vtt
│   ├── lesson2.vtt
│   └── lesson3.vtt
└── images/
    ├── Compare_Adjectives.jpg
    ├── lesson2.jpg
    └── lesson3.jpg
```

## 🖼️ Header Image Guidelines

**Recommended Size:** 1200x675px (16:9 ratio)
**Format:** JPG or PNG
**Max Display Height:** 180px (automatically scaled)

## 📖 VTT Format

Create a `.vtt` file with timestamps:
```
WEBVTT

00:00:00.000 --> 00:00:05.000
First line of text.

00:00:05.000 --> 00:00:10.000
Second line of text.
```

## ✨ Real Example

Current working example:
```
https://speakacademyes.github.io/audios_for_notion/?audio=audio/Compare_Adjectives.mp3&vtt=transcripts/Compare_Adjectives.vtt&title=Comparatives&image=images/Compare_Adjectives.jpg
```

## 🎨 Features

- ✅ Synchronized text highlighting
- ✅ Click any text to jump to that moment
- ✅ Optional header images
- ✅ Clean, professional design
- ✅ Mobile responsive
- ✅ Notion embed optimized
- ✅ No scroll bars in Notion
- ✅ Centered layout

## 🛠️ Customization

The player uses a purple gradient theme with white content cards. Colors and styling can be modified in the `<style>` section of `index.html`.

---

**One player. Infinite lessons. Beautiful headers. Simple.**
