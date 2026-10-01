# 🖼️ Image Watermark Generator

A lightning-fast, client-side web application for stamping text watermarks onto your images. Built with pure HTML5 Canvas and JavaScript—no servers, no uploads, and 100% privacy.

**[👉 Click here to use the App](https://sparktsang.github.io/watermark/)**  

---

## ⚠️ The Problem

Protecting your images with a simple copyright text shouldn't be a hassle, yet the usual methods are deeply flawed:
1. **Desktop Software:** Opening heavy software like Photoshop just to add a line of text is massive overkill.
2. **Online Tools:** Most free online watermark generators require you to upload your high-resolution, private photos to their servers. They are often bloated with ads, compress your images, or compromise your privacy.
3. **Manual Alignment:** Dragging a text box to perfectly align it to a corner (with consistent padding) across 50 different photos is incredibly tedious.

## 💡 The Solution

This tool leverages your browser's native `<canvas>` rendering engine to process images locally. It provides a clean, dark-mode interface where you can configure your watermark once and apply it instantly.

### ✨ Key Features

*   **WYSIWYG Live Preview:** Every adjustment you make—typing text, changing colors, or adjusting margins—updates the preview instantly. No need to click "Apply" or wait for a server response.
*   **Absolute Typography Sizing (pt):** Unlike tools that use confusing relative multipliers, this tool uses standard **absolute point sizes (pt)** (e.g., 24pt, 36pt), giving you the familiar, intuitive control you are used to in word processors. 
*   **Independent X/Y Margins:** Fine-tune your watermark's position with precise, separate controls for horizontal (X) and vertical (Y) distances from the edges.
*   **Auto-Contrast Drop Shadows:** The rendering engine automatically applies a subtle, dynamic drop-shadow to your text. This ensures that white text remains perfectly legible even if placed over bright backgrounds like snow or clouds.
*   **Smart Corner Alignment:** Select a corner (e.g., Bottom-Right), and the tool automatically recalculates the text alignment (`textAlign`). Whether your watermark is 2 words or 20, it will perfectly anchor to the edge without spilling out of the frame.
*   **Smart Export:** Downloaded images are automatically named with precise timestamps (e.g., `watermarked_202610021230.png`) to prevent overwriting your previous files.

---

## 🚀 How to Use

1. **Upload:** Select a local image (PNG, JPEG, WEBP).
2. **Configure Text:** Type your copyright notice (e.g., `© 2026 Spark Tsang`).
3. **Style:** Pick a font (includes the elegant *Abhaya Libre* by default) and color.
4. **Position:** Choose which corner the watermark should anchor to, set your font size (`pt`), and adjust the `X` and `Y` margins for perfect padding.
5. **Download:** Click the download button to instantly save the full-resolution, watermarked image to your computer.

---

## 🛠️ Customizing Your Defaults

Because this tool is built for *your* personal workflow, you can easily change the default settings so you don't have to re-type them every time. 

Simply open `index.html` in any text editor and modify the `value="..."` attributes in the HTML:

*   **Default Text:** Find `<input type="text" id="wmText" value="sparktsang.github.io">` and change it to your actual name or website.
*   **Default Size:** Find `<input type="number" id="wmSize" value="18"` and increase it (e.g., to `60`) if you primarily work with very high-resolution photography.
*   **Default Color:** Find `<input type="color" id="wmColor" value="#ffffff">` and change the hex code.

---

## 🧠 The Philosophy

This tool is a testament to the power of **Zero-Dependency, Client-Side Engineering**. By keeping the codebase contained within a single `index.html` file, it remains infinitely portable, instantly loadable, and completely immune to the privacy risks of the modern web. 

**Fork this repository, tweak the defaults, and take back control of your workflow!**
