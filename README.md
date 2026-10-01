Image Watermark Generator

A client-side image processing tool to instantly stamp text watermarks onto photos.
- **The Problem:** Adding a simple copyright text to an image usually requires opening Photoshop or using sketchy online tools that upload your private photos to external servers. Manually dragging text to align perfectly in the corners is tedious.
- **The Solution:** A lightweight HTML5 Canvas tool. Select an image, type your text, choose a font (includes standard fonts and *Abhaya Libre*), and pick a corner. 
- **Smart Scaling & Rendering:** The tool automatically calculates the optimal font size relative to the image resolution (e.g., `1.3x` scale) and applies a subtle, dynamic drop-shadow so white text remains perfectly legible even against bright backgrounds like clouds or snow. Everything happens instantly in your browser.
