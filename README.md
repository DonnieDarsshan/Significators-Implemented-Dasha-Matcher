# Vedic Significators to Dasha Matcher

A browser-based Vedic astrology tool that visualizes a South Indian style chart, computes KP-style significators, and displays Vimshottari dasha timelines with interactive controls.

This tool is designed for astrologers who want to quickly load Swiss Ephemeris JSON data, analyze significators, and study dasha sequences in a single interface.

---

## Features

### South Indian Kundali

* Dynamic South Indian chart layout.
* Supports:

  * Sign-to-Sign mode
  * KP (0°) mode
  * Vedic (15°) mode
* Custom pivot selection.
* Optional cusp display.

### Significator Engine

* Planet and star-lord based significators.
* Options to include:

  * Conjunct planets
  * Aspects
  * Conjunct cusps
* Split and Split-2 display modes.
* Pivot-based significator rotation.

### Vimshottari Dasha System

* Automatic Mahadasha, Bhukti, and Antara calculation.
* Kannada and English language toggle.
* Month name or numeric date formats.
* Current transit highlighting.
* Date-based dasha finder.
* Adjustable calibration steps.

---

## How to Use

1. Open the HTML file in a web browser.
2. Click **Load Swiss Ephemeris**.
3. Select a Swiss Ephemeris JSON file.
4. The chart and dasha sequence will load automatically.

You can then:

* Change pivot planets.
* Switch between KP, Vedic, or Sign modes.
* Toggle significator options.
* Use the transit finder to locate active dashas.

---

## Required Data Format

The tool expects a JSON file containing:

* Planet longitudes
* Cusp positions
* Lagna
* Birth datetime

Example structure:

```json
{
  "meta": {
    "datetime_utc": "1990-01-01T12:00:00Z"
  },
  "lagna": 123.45,
  "planets": {
    "Surya": 210.12,
    "Chandra": 45.22
  },
  "cusps": {
    "1": 123.45,
    "2": 150.12
  }
}
```

---

## Controls Overview

### Pivot Bar

* Select pivot planet.
* Toggle chart calculation modes.
* Show or hide cusps.

### Significator Options

* Conjunct planets
* Aspects
* Conjunct cuspal points
* Split modes

### Vimshottari Options

* Hide or show dates
* Month names or numbers
* Kannada language toggle

---

## Keyboard-Free Workflow

All interactions are designed to work through on-screen controls:

* Load data
* Toggle options
* Expand dashas
* Find transit dates

---

## Browser Compatibility

Works in modern browsers:

* Chrome
* Edge
* Firefox
* Safari

No installation or server required.

---

## Deployment (GitHub Pages)

1. Create a new repository.
2. Upload the HTML file and this README.
3. Go to **Settings → Pages**.
4. Select the branch (usually `main`).
5. Your tool will be live at:

```
https://yourusername.github.io/repository-name/
```

---

## License

This project is provided as-is for personal and research use.
