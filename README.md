# Live Item Search (DOM Manipulation & XSS Prevention)

A standalone HTML + JavaScript live search implementation built as part of a technical assignment on **Web Security & JavaScript DOM Manipulation**.

## Overview

This project filters an array of items in real time as the user types into a search input, re-rendering the DOM safely without using `innerHTML`.

## Key Features & Implementation Details

- **Real-Time Filtering:** Listens to the `input` event and filters data dynamically with `Array.prototype.filter()`.
- **Safe DOM Rendering:** Builds list elements using `document.createElement()` and assigns text values exclusively through `textContent`.
- **No `innerHTML`:** Avoids `innerHTML` completely to prevent HTML injection and Cross-Site Scripting (XSS) risks when handling user-controlled search queries.

## Project Structure

- `index.html` — Standalone file containing the markup, styling, dataset, search logic, and safe DOM rendering.

## How to Run

1. Clone or download this repository.
2. Open `index.html` directly in any modern web browser (no build step or external dependencies required).
