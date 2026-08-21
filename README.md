# 🧬 GroupDNA: The Group Chat Exposed
![GroupDNA Poster](poster.png)

**"Spotify Wrapped, but to settle debates in the friend group."**

I wanted to see what happens when you apply actual behavioral data analytics to a standard, messy WhatsApp group chat. GroupDNA parses raw chat logs to expose texting habits, sleep schedules, and group dynamics—finally giving us mathematical proof of who the group's biggest "Ghost" is.

### 🚫 The Catch (Constraint-Driven Development)
To make this a real challenge, I banned myself from using high-level data science libraries. This entire engine is built to demonstrate a strict command of core computer science fundamentals:
* **❌ No Pandas:** All data aggregation relies on standard Python dictionaries and hash maps.
* **❌ No Regex (`re`):** The custom parser handles timestamps, multiline continuations, and system alerts using pure algorithmic string manipulation.
* **❌ No Matplotlib:** Temporal activity is rendered directly in the terminal via an ASCII-powered NumPy matrix.

## ⚙️ What It Actually Does

* **Custom Chat Parser:** Strips out system alerts and `<Media omitted>` tags to build a clean pipeline of valid messages.
* **The 24-Hour Heatmap:** Uses an N x 24 dimensional `NumPy` array to build an activity matrix, exposing exactly when each person is actually awake.
* **Vocabulary Vibe Check:** Filters out standard punctuation and stop-words to track the group's most heavily used slang.
* **Personality Archetyping:** Calculates average response speeds and silent streaks to assign rule-based behavioral personas (e.g., *The Spammer*, *The Night Owl*, *The Ghost*).

## 🚀 Try It on Your Own Friends

1. Export a WhatsApp chat without media.
2. Rename the exported text file to `#your_own_chatfile`.
3. Drop it in the same directory as the script.
4. Run the Python notebook to generate your terminal dashboard.

## 👨‍💻 Built By
**Atharv Mandekar**  
*Undergraduate, Computer Science & Engineering | Symbiosis Institute of Technology*

Usually, I am deep into cybersecurity SOC operations or building full-stack MERN applications, but sometimes the best way to practice pure coding fundamentals is to analyze your own friends.
