# Simple Grid Calculator

A clean, responsive calculator web application built with semantic HTML5, CSS Grid layout, and vanilla JavaScript. This project marks my **very first official JavaScript application**, focusing on DOM manipulation, event handling, and array methods.

---

## 🛠️ Tech Stack & Features

* **HTML5:** Semantic structure using input elements for display data and custom `data-*` attributes for passing values.
* **CSS3 (Grid & Flexbox):** Centralized layout utilizing Flexbox on the body, combined with a precise 4-column **CSS Grid** to handle the responsive button arrangement. Features modern active state scaling effects for a tactile button-press feel.
* **Vanilla JavaScript:** Employs programmatic event listening (`forEach` loops), dynamic string token parsing, conditional switch structures, and layout state rendering.

---

## 🧠 How the JavaScript Works

The JavaScript file acts as the controller that bridges the HTML layout with mathematical logic. Here is a quick look under the hood of what I implemented:

1.  **DOM Selection:** Uses `querySelector` and `querySelectorAll` to grab the interactive elements from the page.
2.  **Event Delegation:** Instead of manually writing 20 individual click handlers, the script uses a `.forEach()` loop to iterate through every button and attach a single programmatic event listener.
3.  **Data Management:** Uses HTML `data-value` attributes to cleanly pass clicked symbols or digits into the background execution string (`let output`).
4.  **Edge-Case Protection:** Includes logic to detect if the string is empty, blocking operators (like `*`, `/`, or `%`) from being selected first and crashing the sequence.
5.  **Dynamic Rendering:** Updates the HTML input's `.value` attribute in real-time, instantly pushing memory calculations to the user's view.

---

## 📂 Project Structure

```text
├── index.html   # Application structure and button grids
├── calc.css     # Styling, layouts, color palette, and micro-interactions
└── calc.js      # Application state engine and mathematical operations
