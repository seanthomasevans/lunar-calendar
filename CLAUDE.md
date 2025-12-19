# Lunar Calendar

Hebrew lunar calendar visualization with Kabbalistic elements for Toronto.

## Overview

A contemplative moon-centric display showing:
- 3D moon with accurate astronomical phase rendering
- Hebrew date (gematria) with phonetic transliteration
- Contextual Kabbalistic quotes (Chanukah, Shabbat, moon phase)
- Weather data from OpenWeatherMap
- Zmanim (candle lighting, havdalah) on Shabbat

## Tech Stack

- **Three.js** - 3D moon rendering with NASA textures
- **@hebcal/core** - Hebrew calendar calculations
- **Canvas 2D** - Background, particles, fallback moon
- **OpenWeatherMap API** - Weather data

## Design

Dieter Rams / Braun aesthetic:
- Clean, functional typography
- All caps labels with wide letter-spacing
- Neutral dark blue background
- Minimal UI elements

## Running Locally

```bash
cd /Users/seanthomasevans/workspace/lunar-calendar
python3 -m http.server 8080
open http://localhost:8080
```

## Location

Toronto (43.6532°N, 79.3832°W)

## Key Files

- `index.html` - Complete app (HTML, CSS, JS)
- `assets/moon_texture_4k.jpg` - NASA moon surface texture
- `assets/moon_bump_4k.jpg` - Moon bump map for 3D depth

## Features

### Quote System (Priority Order)
1. **Chanukah** - Night-specific quotes (1-8)
2. **Shabbat** - Friday/Saturday quotes
3. **Moon Phase** - Kabbalistic meaning by lunar day

### Moon Phase Calculation
Uses January 6, 2000 new moon (JD 2451550.1) as reference with synodic month of 29.530588853 days.
