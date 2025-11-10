# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a web-based studio assistant tool called "Derbyshire" that helps with music production calculations including reverb/delay timing, pitch/tempo relationships, and audio math. It's a single-page application built with vanilla HTML, CSS, and JavaScript.

## Architecture

The application is structured as a single HTML file (`src/index.html`) containing:

- **HTML Structure**: Tabbed interface with 5 main sections:
  - Timing & Effects (tempo-based timing calculations, delay effects, rhythm/groove)
  - Sampling & Pitch (pitch-tempo conversions, audio math)
  - Music Theory (key/scale tools, harmonic mixing)
  - Technical (audio technical specs, frequency analysis, hardware sync)
  - References (quick reference tables for audio formats, tunings, impedance)

- **CSS Styling**: Modern glassmorphism design with:
  - Dark gradient background
  - Semi-transparent cards with backdrop blur
  - Responsive grid layout
  - Purple/blue gradient accent colors
  - Mobile-responsive breakpoints

- **JavaScript Functionality**: Vanilla JS with calculator functions for:
  - Tempo-based timing calculations
  - Pitch/frequency conversions
  - Audio math (dB to gain, cents to ratio, sample rate conversions)
  - Music theory calculations (key detection, scale generation)
  - Room acoustics and hardware sync calculations

## Key Features Implemented

Current working features include:
- Tempo-based timing calculator for reverb/delay
- Pitch/tempo relationship calculators for sampling
- Dotted delay and ping-pong delay timing
- Multi-tap delay patterns
- BPM to Hz conversion for LFO sync
- Cents to frequency ratio calculations
- dB to gain ratio calculator
- Sample rate conversion ratios
- Key detection and harmonic mixing
- Swing timing calculations
- Polyrhythm calculations
- Room mode calculations
- MIDI clock and hardware sync timing

## Development Notes

- No build process required - this is a static HTML file
- No package.json or dependencies - uses only vanilla web technologies
- No testing framework configured
- The application is fully self-contained in a single file
- Uses modern ES6+ JavaScript features
- Responsive design works on mobile and desktop

## File Structure

```
/
├── README.md           # Project documentation with feature roadmap
├── src/
│   └── index.html     # Main application file (HTML + CSS + JS)
└── LICENSE            # MIT License
```

## Planned Features (from README)

The README.md contains an extensive TODO list of potential features organized by category:
- Additional delay/echo features
- Key/scale tools (circle of fifths, mode calculator)
- MIDI/technical tools (note to frequency conversion, buffer size calculator)
- Rhythm tools (groove templates)
- Sampling helpers (loop length, crossfade timing)

When adding new features, follow the existing patterns:
1. Add HTML structure within the appropriate tab
2. Style using the existing CSS classes and design system
3. Implement calculation logic as standalone JavaScript functions
4. Call calculations both on input events and during page load
5. Update results in real-time as user types