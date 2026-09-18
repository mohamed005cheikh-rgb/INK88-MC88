<div align="center">

# ✒️ INK88

**A quiet archive for ASCII art — write it in a text file, watch it appear.**

</div>

---

## 👋 Welcome

Most websites that showcase ASCII art bury it under layers of JavaScript, animation libraries, and loading spinners. The art itself is barely visible by the time the page finishes deciding how it wants to look.

INK88 takes the opposite path. It has no framework. No dependencies. No build step. It reads a single text file, splits it on a line of three dashes, and shows you what's inside. Every artwork gets an ID, a place on the page, and a copy button — nothing more. The whole design is borrowed from an old paper catalog: cream background, thin rules between rows, a Times New Roman serif for the labels, and `Courier` for the art itself, where it belongs.

This matters because ASCII art deserves a page that gets out of its way. You drop a new piece into `artworks.txt`, separate it with `---`, and it's on the archive the next time you refresh. No database, no CMS, no admin panel. Just text, loaded as text, displayed as text.

Open it and see for yourself — scroll through, find something you like, hit **Copy**, and paste it wherever you want. That's the entire interaction.

---

## 📸 Look Inside

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/INK88-MC88/raw/main/images/preview-1.png" alt="The INK88 archive homepage" width="100%" />
  <br />
  <sub><b>① The archive</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/INK88-MC88/raw/main/images/preview-2.png" alt="A single artwork row with copy button" width="100%" />
  <br />
  <sub><b>② A single row, ready to copy</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/INK88-MC88/raw/main/images/preview-3.png" alt="INK88 on mobile" width="100%" />
  <br />
  <sub><b>③ The same archive, on a phone</b></sub>
</div>

---

## ✨ What you'll find

**The whole archive lives in one text file.**  
Every drawing is stored in `artworks.txt`, separated by a line of three dashes: `---`. That's the only rule. You can write art in your editor of choice, paste it in, and it will show up. No HTML to hand-craft. No markup to learn. Just the art, as it is.

**A vintage paper aesthetic that stays out of the way.**  
The background is a warm cream. The container is off-white with a soft shadow. The header is set in Times New Roman with wide letter-spacing, lowercase, unapologetic. Every row has a thin rule between it and the next one. The `Courier` monospace sits inside each row so the art keeps its exact shape. Nothing is trying to look modern. The design is here to frame the art, not to compete with it.

**Numbered entries, from `#001` upward.**  
Every artwork gets an automatic ID in the left column — `#001`, `#002`, `#003`. If you add new art to the middle of the file, the numbers shift automatically. No manual bookkeeping, no risk of skipping a number, no duplicate IDs.

**One copy button per artwork.**  
Each row has a small outlined **Copy** button in the right column. Click it and the entire artwork — every space, every line break, every character — goes straight to your clipboard. The button confirms with a quiet **Copied!** for a moment, then returns to normal. No modal, no toast, no interruption.

**Responsive without breaking the art.**  
On a wide screen, each row is three columns: ID, artwork, button. On a phone, those columns fold into a single stack — the ID above, the art in the middle, the copy button below. Crucially, the `pre` block scrolls horizontally on small screens instead of wrapping, so a wide drawing never gets its characters shifted to the wrong line.

**Nothing loads if it shouldn't.**  
If `artworks.txt` is missing or the browser can't reach it, INK88 shows a single clear line: *"Could not load artworks.txt. Make sure you are running this via a local server or GitHub Pages."* No blank page, no console error as the only clue. Just the truth, in the same voice as everything else here.

**No tracking, no analytics, no backend.**  
It's a single HTML file that reads a single text file. There is nothing else. Your clipboard never leaves your device. The archive never phones home. You can open it entirely offline — as long as the text file sits next to it.

---

## 🧭 How it works

**1. Put `index.html` and `artworks.txt` in the same folder.**  
That's the entire project. Two files, side by side.

**2. Open the page.**  
Because the page loads the text file with `fetch`, it must be served by a real server. Opening the HTML file directly with `file://` will fail on most browsers. GitHub Pages, a small local server, or any static host will work.

**3. See the archive.**  
Each artwork is loaded in order, numbered, and displayed inside a cream catalog.

**4. Copy what you like.**  
Click **Copy** on any row. Paste the art wherever you want — a text file, a comment, a chat, a document.

**5. Add new art.**  
Open `artworks.txt`, scroll to the bottom (or anywhere you like), and paste your new drawing. Separate it from the previous one with a line of three dashes:

Refresh the page. Your new artwork is now part of the archive.

**6. Delete what you don't want.**  
Remove the artwork and its separator from `artworks.txt`. Refresh. Gone.

That's the whole loop. Nothing to learn.

---

## 🛠️ A few small helps

**"The page says it can't load `artworks.txt`."**  
That usually means you opened `index.html` directly by double-clicking it, so the browser is using the `file://` protocol — and `fetch` refuses to read local files that way. Run it from a small server (`python3 -m http.server`, or any static host like GitHub Pages), and it works immediately.

**"My art is showing on the wrong lines."**  
Check that every line inside `artworks.txt` uses the **same kind of space** — mixing regular spaces with non-breaking spaces will shift things. Also make sure you're not using tabs where you meant spaces. The `pre` block preserves exactly what you wrote, so the file needs to match the intent.

**"The separator isn't working."**  
The separator must be a line that contains **only** three dashes (`---`) and nothing else — no leading spaces, no trailing text. If your editor auto-inserts a space, remove it. `---` on its own line is the only valid form.

**"Copy puts the wrong thing on my clipboard."**  
The copy button grabs the artwork exactly as it appears in the text file — including blank lines at the start or end if they're there. If you see extra empty lines when you paste, go back to `artworks.txt` and trim them; the page will mirror whatever the file contains.

**"The art is too wide on my phone."**  
The `pre` block is set to scroll horizontally instead of wrapping, so wide drawings stay intact. Swipe left and right inside the row to see the whole thing. That's intentional — wrapping would destroy the alignment.

**"Can I add images or colors?"**  
Not in this version. INK88 is deliberately about *text* art — the whole aesthetic depends on that. Adding images or colors would break the mood that makes it work.

**"Does anything track me when I copy?"**  
No. The copy action calls `navigator.clipboard.writeText()` directly in your browser. Nothing goes to a server. There is no server.

**"Can I rename the file from `artworks.txt`?"**  
Yes — just update the filename in the JavaScript where it does `fetch('artworks.txt')`. Everything else works the same.

---

<div align="center">

### 📞 A question, an idea, a bug?

[![Email](https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white)](mailto:mohamed005cheikh@gmail.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-+222_30_73_64_75-25D366?style=flat-square&logo=whatsapp&logoColor=white)](https://wa.me/22230736475)
[![GitHub](https://img.shields.io/badge/GitHub-mohamed005cheikh--rgb-181717?style=flat-square&logo=github)](https://github.com/mohamed005cheikh-rgb)

<br />

*Write in text. Read in text. Nothing more.*

<sub>© 2026 Mohamed Cheikh — MC88</sub>

<br />
<br />

    ███    ███    ████████    ████████    ████████
    ████  ████   ███    ███  ███    ███  ███    ███
    ██ ████ ██   ███         ███    ███  ███    ███
    ██  ██  ██   ███          ████████    ████████
    ██      ██   ███         ███    ███  ███    ███
    ██      ██   ███    ███  ███    ███  ███    ███
    ██      ██    ████████    ████████    ████████

</div>
