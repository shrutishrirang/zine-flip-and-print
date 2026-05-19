# 📖 zine flip & print.

A local, client-side web application to preview, customize, and impose an **8-page folding booklet (zine)** onto a single sheet of A4 paper.

---

## ✂️ Folding & Cut Scheme

```text
+-----------------------------------+
|  pg 7  |  pg 6  |  pg 5  |  pg 4  |  (Inverted 180° for folding)
|--------+--------+--------+--------|
|  back  | front  |  pg 2  |  pg 3  |  (Right side up)
+-----------------------------------+
```
1. **Fold:** Fold in half horizontally, then fold vertically into booklet panels.
2. **Cut:** Slit the horizontal center crease between page columns 2-3, then collapse into booklet pages.

---

## ✨ Key Features

*   **📖 Tactile Zine Previewer:** Simulates a physical zine layout with realistic fold shadows.
*   **🔀 Drag-and-Drop Reordering:** Smooth layout rearrangement with mobile touch gesture support.
*   **⬆️ Bulk Upload Drop Zone:** Drop 8 files at once; auto-sorts them alphabetically by filename.
*   **⚙️ Intelligent Preprocessing:** Auto center-crops to A4 portrait ratio and handles EXIF orientation rotation.
*   **🎨 Dynamic Backdrop Customizer:** Set colors and render vector textures (*Gingham, Dots, Stripes, Herringbone*) on high-DPI canvases.
*   **🖨️ Double-Sided PDF Prints:** Exports imposed pages with folding cut lines plus optional backside design.

---

## 🛠️ Technical Details & Stack

*   **Front-End:** Vanilla HTML5, CSS3, and JavaScript—runs completely client-side.
*   **Libraries:** Uses [jsPDF](https://github.com/parallax/jsPDF) for vector booklet creation and [html2canvas](https://html2canvas.hertzen.com/) for high-DPI screenshots.
*   **Imposition Layout:** Imposes `pages[0-7]` dynamically. Rotates top row 180° so folded panels stand upright.

---

## ⚡ How to Run

1. **Locally:** Double-click [index.html](file:///Users/shrutikulkarni/Documents/codework/zine_flipbook/index.html) in your browser.
2. **Deploy:** Fully static and perfectly suited for free hosting on **GitHub Pages**.

---
*Handcrafted for designers, zinesters, and print-lovers everywhere. 🖤*
