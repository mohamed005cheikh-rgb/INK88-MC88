<div align="center">

# ✒️ INK88

**A quiet archive for 1-bit text art — drop a file in the folder, watch it come alive.**

</div>

---

## 👋 Welcome

Most digital archives of text art bury their contents under heavy JavaScript frameworks, complex routing, and bloated loading screens. By the time the page finally renders, the art itself has lost its raw, minimalist impact.

INK88 takes the opposite, purist path. It operates with no external framework, no heavy dependencies, and no manual list maintenance. Instead of parsing a single monolithic file, it reads directly from a dedicated `art` folder, loading individual artwork files sequentially (`1.txt`, `2.txt`, and so on) until the archive concludes. 

Every artwork is framed within an old paper catalog aesthetic: a warm cream background, delicate thin rules, a classic serif font for labels, and `Courier Prime` monospace for the art where it belongs. Accompanied by an elegant 6-second quill animation upon entry, INK88 gets entirely out of the way, letting the 1-bit text art speak for itself.

---

## 📸 Look Inside

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/INK88-MC88/raw/main/images/preview-1.png" alt="The INK88 archive homepage" width="100%" />
  <br />
  <sub><b>① The archive and vintage catalog</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/INK88-MC88/raw/main/images/preview-2.png" alt="A single artwork row" width="100%" />
  <br />
  <sub><b>② A single catalog row with classic framing</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/INK88-MC88/raw/main/images/preview-3.png" alt="INK88 on mobile" width="100%" />
  <br />
  <sub><b>③ The same archive, viewed on a mobile device</b></sub>
</div>

---

## ✨ What you'll find

**An organized `art` folder structure.** Instead of packing everything into one massive file, the archive lives inside a dedicated `art` folder. Each piece of art has its own clean text file (`1.txt`, `2.txt`, `3.txt`, etc.). The smart sequential loader detects and displays them automatically in order. Adding new art is as simple as dropping a new numbered text file into the folder.

**A 6-second poetic splash screen.** Upon opening the archive, an elegant SVG quill animation draws itself across a parchment canvas, accompanied by classic typography. You can watch the art unfold or simply click anywhere to skip directly into the gallery.

**A timeless vintage paper aesthetic.** The background simulates warm vintage parchment. The container features soft shadows and subtle corner ornaments. Headings use classic serif typography with wide letter-spacing, while the art itself is safely bound in `Courier Prime` monospace to protect its exact alignment and shape.

**Numbered entries, from `#001` upward.** Every artwork receives an automatic, elegant catalog number in its header (`#001`, `#002`, `#003`...), derived directly from its file index. No manual bookkeeping or ID management required.

**Copy feature under maintenance.** The clipboard copy functionality is currently undergoing maintenance and improvements to ensure a flawless experience, and will return in the very near future, Insha'Allah. Meanwhile, enjoy browsing and downloading your favorite pieces freely.

**Responsive layout protecting pixel alignment.** On widescreen monitors and mobile devices alike, the layout adapts gracefully. The `pre` block scrolls horizontally on smaller screens rather than wrapping lines, ensuring that wide drawings never suffer from character displacement.

**Zero overhead, zero tracking.** INK88 requires no database, no backend CMS, and no tracking scripts. It is a lightweight, pure static experience that respects your privacy and can run seamlessly anywhere.

---

## 🧭 How it works

**1. Set up your workspace.** Ensure your `index.html` file sits alongside an `art/` folder in your project directory.

**2. Populate the `art` folder.** Place your 1-bit text art inside individual text files named sequentially (`1.txt`, `2.txt`, `3.txt`, etc.) inside the `art` folder.

**3. Launch the archive.** Open the page via a local server (`python3 -m http.server`, Live Server) or deploy it instantly on GitHub Pages. Direct `file://` opening is blocked by modern browser security policies for local fetches.

**4. Experience the welcome screen.** Watch the 6-second quill animation render or click anywhere on the screen to enter the gallery immediately.

**5. Add new art effortlessly.** Whenever you create a new piece, simply save it as the next sequential number (e.g., `4.txt`) inside the `art` folder and push or refresh. The engine will pick it up automatically.

---

## 🛠️ Frequently Asked Questions

**"The page says it cannot load the art files."** Make sure you are running the project through a local development server or static host like GitHub Pages rather than double-clicking `index.html` directly, as browsers restrict local file access (`file://`).

**"How do I add a new artwork?"** Just create a new text file inside the `art` folder named with the next consecutive number (e.g., `3.txt`) containing your 1-bit art, and refresh your browser.

**"My art formatting looks misaligned."** Ensure your text files use consistent spacing and avoid mixing tabs with spaces. The `pre` element preserves exact whitespace characters.

**"When will the copy button return?"** The copy feature is currently under active maintenance and will be restored very soon, Insha'Allah.

**"Can I customize the folder name?"** Yes, you can modify the folder path inside the JavaScript fetch logic if you prefer a different directory name.

---

<div align="center">

### 📞 Questions, ideas, or feedback?

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

