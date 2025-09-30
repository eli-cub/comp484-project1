# LA Kings Fan Page – Project Documentation

## Overview

This project is a multi-page fan site for the Los Angeles Kings NHL team. It demonstrates the use of several HTML5 elements and attributes, including `<data>`, `<area>`, `<iframe>`, `<value>`, `<coords>`, and `<sandbox>`. Below is a summary of where and how each is used.

---

## HTML Elements & Attributes Used

### 1. `<data>` and `value`
- **Where:** [`roster.html`](roster.html)
- **How:** Used in the roster tables to semantically mark up player numbers and stats.
- **Example:**
  ```html
  <td><data value="11">11</data></td>
  <td><data value="1454">1454</data></td>
  ```
  The `value` attribute provides a machine-readable version of the data for each player stat.

---

### 2. `<area>` and `coords`
- **Where:** [`media.html`](media.html)
- **How:** Used in an image map to make different sections of the arena map clickable, each linking to a different seating level.
- **Example:**
  ```html
  <area shape="rect" coords="183,7,423,53"
        href="https://aviewfrommyseat.com/venue/Crypto.com+Arena/level/8/Level+300/"
        alt="300 Level" title="300 Level" target="_blank">
  ```
  The `coords` attribute defines the clickable area on the image.

---

### 3. `<iframe>` and `sandbox`
- **Where:** [`index.html`](index.html) and [`media.html`](media.html)
- **How:** Used to embed external content such as Google Maps and YouTube videos.
- **Example (Google Maps):**
  ```html
  <iframe
    title="Map – Crypto.com Arena"
    src="https://www.google.com/maps?q=Crypto.com+Arena&hl=en&z=15&output=embed"
    width="600" height="450"
    loading="lazy"
    referrerpolicy="no-referrer-when-downgrade"
    sandbox="allow-scripts allow-same-origin allow-presentation"
    allowfullscreen>
  </iframe>
  ```
  The `sandbox` attribute restricts the iframe’s capabilities for security.

---

## File List

- [`index.html`](index.html): Home page with team intro and embedded Google Map.
- [`roster.html`](roster.html): Team roster and stats using `<data>`.
- [`media.html`](media.html): Media highlights and interactive arena map using `<iframe>` and `<area>`.
- [`history.html`](history.html): Team history, logos, and uniforms.
- [`styles.css`](styles.css): Site styling.

---

## Author

Eli Cubillo  
&copy; 2025 LA Kings Fan Page
