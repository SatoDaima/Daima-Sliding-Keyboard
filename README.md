# Daima-Sliding-Keyboard
Interactive demo of Daima — an Android keyboard with a triangle-based QWERTY layout, gesture-driven backspace joystick, cursor control, quick-access symbol buttons, and more.

---

**An Android keyboard that reimagines how we type with our thumbs.**

🔗 **[Try the interactive demo](https://satodaima.github.io/Daima-Sliding-Keyboard)**

---

## What is Daima?

Daima is an Android keyboard (IME) in development, designed to replace Gboard/Samsung Keyboard with a more precise, accessible, and gesture-driven typing experience. Its most distinctive feature is a **triangle-based QWERTY layout** where two letters share each triangle, combined with a rich gesture system that keeps your thumbs in the home position.

---

## ✅ What the demo already does

**QWERTY with triangles and secondary symbols**
Traditional keyboards have small, tightly packed keys — easy to miss if you have large thumbs or need extra precision. Daima's solution: each row is divided into large triangles, giving each letter a much bigger hit area. A 2D heat map system (coming soon) will further improve accuracy by calculating the probability of each nearby letter based on where your finger actually lands. Each key also has a secondary symbol visible in its corner — swipe up to insert it instantly, without switching panels.

**Backspace joystick**
Press and hold briefly (less than 500 ms), then slide left to delete. Speed increases progressively the further you go. Slide right to recover deleted text — character by character, at the same speed.

**Oversized Enter key — no Backspace**
Backspace key was intentionally removed to make room for a much larger Enter key. On standard keyboards, Enter is easy to miss; on Daima it's impossible to miss. Backspace was replaced by a quick swipe left gesture (swipe right to undo) — faster and more natural once you get used to it.

**Precision magnifier (long press)**
Press and hold any letter key for 500ms without moving. A red circular area appears over your touch point. While your finger moves, the top suggestion row shows the detected letter in real time. Release to insert it — designed for users who need extra precision.

**Mini editor (Row 1)**
An optional row you can show or hide depending on the app. Designed for spell and grammar checking — it displays your full text before sending, with wavy underlines for spelling errors (red) and grammar issues (orange). The cursor is always visible and repositionable. Most useful in Gmail, Docs or any long-form writing app; easy to hide in WhatsApp or similar.
Note: spell and grammar checking requires internet connection and is not yet active in this demo.

**Cursor control**
Press and hold the spacebar, then drag in any direction to move the cursor — like a trackpad. Works across the full keyboard area.

**Symbol panel with 3 layers**
Like any keyboard, but with a twist: in the first layer you can swipe ↑ on any key to get the second-layer symbol directly, without switching layers.

**Two quick-access symbol buttons**
One button on each side of the spacebar, each with two symbols (tap for one, swipe up for the other). Long press opens a panel of 12 additional symbols. Both buttons are fully customizable — swap any of the 12 symbols with your preferred ones, including Unicode.

**Emoji panel**
Swipe up from the spacebar. 10 full Unicode categories with arrow-based navigation.

**Smart clipboard**
Two columns: recent (auto-deleted after 12 hours) and pinned (permanent). Edit mode lets you organize, pin, and delete clips.

**Dynamic word suggestions**
The suggestion row adapts in real time as you type. Instead of always showing a fixed number of options, the local AI model determines how many relevant suggestions to display based on context — showing fewer when the word is unambiguous, and up to 10 when multiple candidates are likely. Only suggestions above a confidence threshold are shown.

---

## 🚧 In development

**2D heat map for key precision**
On touch, the system will calculate the probability of each nearby letter based on distance from the touch point, improving accuracy especially at triangle edges.

**Word suggestions while you type**
Row 2 will show real-time predictions from a local language model — no API, no internet required, no latency.

**Spell and grammar checking**
Wavy underlines in Row 1 for spelling (red) and grammar (orange) errors, powered by LanguageTool.

**Emoji search in Spanish and English**
Type "corazón" and see related emojis. Local Unicode CLDR database, works offline.

**Swipe typing**
An additional layer where you form words by sliding your finger between letters.

**Dark mode**

**Translation** across all keyboard layers

---

## Status

> This is an **interactive HTML demo** — not the final Android app. The demo runs in any desktop browser and simulates the keyboard experience. The Android (Kotlin) implementation is planned as the next phase.

---

## About

Designed and developed by **Lauren** ([@SatoDaima in X] (https://github.com/SatoDaima))  
Built with HTML, CSS and vanilla JavaScript — no frameworks, no dependencies.
