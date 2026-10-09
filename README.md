# Lista e Pazarit: Shopping List

A lightweight shopping-list / to-do app in vanilla JavaScript, with an Albanian UI (*"Lista e Pazarit"*, "shopping list"). Items persist in the browser through `localStorage`, so the list is still there after a reload.

**Live demo:** https://rexhinokovaci.github.io/todojs/

## Features

- Add an item with the **+** button or by pressing **Enter** (empty input is ignored)
- **Edit** an item in place: the first click unlocks the field, the second click saves it
- **Remove** an item
- The list is stored as JSON in `localStorage` under the key `todos`, and restored on load
- Starts with two sample items ("Kafe", "Oriz") that show the layout

## How it works

Each list entry is created by a small `item` class in `index.js`. It builds the DOM for the row (a read-only input plus EDIT/REMOVE buttons) and keeps the `todos` array in `localStorage` in sync on every add, edit and remove.

## Tech stack

HTML, CSS (Google Fonts "Hind") and vanilla JavaScript. Font Awesome supplies the icon. No build step. Hosted on GitHub Pages.

## Running locally

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

---

Built by [Rexhino Kovaci](https://github.com/rexhinokovaci) — DevOps & AI engineer in Tirana, Albania. Need an app built? [Get in touch](mailto:kovacirexhino@gmail.com).
