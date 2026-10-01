# AUPP Trading Club — Master Slide Deck Design & Creation Guidelines

This document is the official design standard and implementation blueprint for creating presentation slides for the **AUPP Trading Club** (American University of Phnom Penh). 

Whenever you prompt an AI (Antigravity, Claude, ChatGPT, Gemini, etc.) to create a new presentation deck for this club, provide or reference this document to ensure 100% brand consistency, visual excellence, and teaching quality.

---

## 🏛️ 1. Club Identity & Brand System

### 1.1 Colors
The color palette reflects institutional finance, academic authority, and clean modern aesthetics:

| Role | Color Name | HEX Code | Usage |
|---|---|---|---|
| **Primary Navy** | Oxford Deep Navy | `#0D1F3C` / `#102A43` | Main headings, cover background accents, card headers, dark text |
| **Secondary Navy** | Steel Navy | `#1A3258` | Subheadings, active states, border accents |
| **Primary Accent** | Crimson Red | `#C8102E` / `#B81D24` | Accent underline bars, key numbers, warning badges, bear candles |
| **Accent Soft Red** | Crimson Tint | `#FDE8EA` / `#FEE2E2` | Callout box backgrounds, negative badge backgrounds |
| **Bullish Green** | Emerald Growth | `#00A868` / `#00B074` | Bullish candlesticks, success checkmarks, valid signals |
| **Bullish Soft Green** | Mint Tint | `#E6F7F0` | Bullish card badges, discount zone highlight |
| **Neutral Blue** | Royal Blue | `#2563EB` | HTF trajectory lines, informational callouts |
| **Slide Background** | Pure White | `#FFFFFF` | Slide background canvas |
| **Card / Section Bg** | Off-White Slate | `#F8FAFC` / `#F4F6F9` | Secondary cards, callout containers, thumbnail cards |
| **Card Borders** | Soft Gray | `#E2E8F0` / `#E5E9F0` | Card borders, table dividers |
| **Body Text** | Charcoal | `#2D3748` / `#334155` | Body copy, bullet explanations |
| **Muted Text** | Slate Muted | `#5A6A80` / `#718096` | Subtitles, slide counter, footer metadata |

### 1.2 Typography
Always use the following Google Fonts:

- **Headings & Titles**: `'Cinzel', serif` (Weights: 600, 700, 800)
  - Uppercase or Title Case with slight tracking (`letter-spacing: 0.03em` to `0.05em`).
  - Gives a prestigious, Wall Street / institutional financial feel.
- **Body, Badges & Labels**: `'Montserrat', sans-serif` (Weights: 400, 500, 600, 700, 800)
  - Modern, geometric, clean, and highly readable on lecture hall projectors.

### 1.3 Signature Visual Elements
Every content slide must follow these signature brand motifs:
1. **Title Underline Bar**: A 70px wide, 4px high crimson red pill bar (`background: #C8102E; border-radius: 2px; margin-top: 12px; margin-bottom: 24px;`) directly below the main slide heading.
2. **Top Right Logo**: The horizontal club logo (`assets/horizontal.png` or `../Asset/horizontal.png`) positioned neatly in the slide header.
3. **Slide Footer**: A clean bottom rule with:
   - Left: `AUPP TRADING CLUB • [TOPIC / SERIES]`
   - Right: Current topic title + pill badge with 2-digit slide number (e.g. `07`).
4. **Numbered Step / Card Badges**: Large serif numeral (`01`, `02`, `03`) in crimson red or navy above card titles.
5. **Key Message Quotes**: An italicized summary pill (`padding: 14px 20px; background: #EDF2F7; border-radius: 8px;`) with a bold crimson `Key Insight:` or `Rule of Thumb:`.

---

## 📐 2. Canvas & Technical Format

- **Aspect Ratio**: Standard 16:9 Widescreen (`1440px × 810px` native internal canvas).
- **Technology Stack**: Native HTML5, Vanilla CSS3, and modern JavaScript (no heavy runtime framework required).
- **Charts & Visuals (Candlesticks + Line Graph)**:
  - Technical charts MUST display **BOTH real Japanese candlesticks** (green bullish and red bearish bodies with wicks) **AND the structural line graph** overlaying/connecting the swing points (Low, High, HL, HH, LH, LL, BOS, MSS).
  - Include view toggle tabs on the chart container: `[Both (Candles + Line)]`, `[Candlesticks]`, `[Line Only]` with "Both" active by default.
- **Responsive Auto-scaling**: Center and scale the 1440×810 stage via CSS `transform: scale(...)` based on viewport width/height, maintaining the exact 16:9 ratio with zero layout breakage or overflow.
- **Navigation Engine**:
  - `ArrowRight` / `Space` / `PageDown` / `J` → Next slide.
  - `ArrowLeft` / `PageUp` / `K` → Previous slide.
  - `Home` / `End` → First / Last slide.
  - `F` → Toggle Fullscreen presentation mode.
  - `G` → Slide Grid Overview Modal (allows quick jumping to any slide).
  - `P` / `Cmd+P` → 1-Click Export to PDF.
- **Print / PDF Export Support**: Pre-configured `@media print` with `@page { size: 16in 9in landscape; margin: 0; }` ensuring each slide prints cleanly to a single page without UI controls.

---

## 📚 3. Standard Presentation Structure

Keep the slides beginner-friendly, clean, and digestible (12–15 slides max). Do not overwhelm beginners with overly dense institutional jargon unless requested:

1. **Slide 1: Cover Page** — Circular badge logo (`assets/logo.png`), Topic, Subtitle, "Organized by AUPP Trading Club • Supported by AUPP".
2. **Slide 2: Introduction / Hook** — Simple definition & big picture concept.
3. **Slide 3: Table of Contents** — 5–6 clear workshop topics with numbered crimson badges (`01`–`06`).
4. **Slide 4: Club Disclaimer** — Standard AUPP educational and risk disclaimer.
5. **Slide 5: Core Categories / Trends** — e.g. Uptrend, Downtrend, Sideways.
6. **Slide 6: Key Definitions / Abbreviations** — Core terms (e.g. HH, HL, LH, LL).
7. **Slides 7–9: Detailed Visual Breakdowns** — Clean, simple SVG price wave diagrams showing each scenario in action.
8. **Slide 10: Trend Continuation (e.g., BOS)** — Simple explanation and visual diagram.
9. **Slide 11: Trend Reversal (e.g., Market Structure Shift / MSS)** — Simple explanation and visual diagram.
10. **Slide 12: Quick Class Practice** — Interactive chart diagram with toggle buttons to reveal answers in class.
11. **Slide 13: Summary Key Takeaways & Q&A** — Bullet checklist and discussion closing.

---

## 🤖 4. Copy-Paste Master Prompt for AI

Whenever you ask **this AI** or **any other AI** (ChatGPT, Claude, etc.) to generate another presentation deck, copy and paste the prompt template below:

```text
You are an expert financial educator and frontend presentation designer. I need you to create a complete, presentation-ready HTML/CSS/JS slide deck for the "AUPP Trading Club" (American University of Phnom Penh).

TOPIC TO TEACH: [INSERT YOUR TOPIC HERE, e.g., "Liquidity & Order Blocks" or "Fibonacci & Premium/Discount Zones"]

TARGET AUDIENCE: University students, aspiring traders, and club members.

DESIGN & BRAND REQUIREMENTS:
1. Color Scheme:
   - Primary Navy: #0D1F3C (Dark text, headers, accents)
   - Secondary Navy: #16284F
   - Accent Crimson: #C8102E (Title underline bars, warning tags, bearish markers)
   - Bullish Green: #00A868 (Bullish candles, success badges)
   - Background: Crisp #FFFFFF with #F8FAFC card backgrounds and #E2E8F0 borders.
2. Typography:
   - Headings: 'Cinzel', serif (Weights 600, 700, 800) with letter-spacing
   - Body & Badges: 'Montserrat', sans-serif (Weights 400, 500, 600, 700)
3. Signature Elements:
   - Every slide title must have a 70px x 4px crimson underline bar (#C8102E).
   - Use 'assets/horizontal.png' in the top right header of every slide.
   - Use 'assets/logo.png' on the cover slide and closing slide.
   - Include the official slide footer: "AUPP Trading Club • [Series Name]" on left, Topic and 2-digit slide counter badge on right.
4. Layout & Technical Format:
   - 16:9 widescreen format (1440px x 810px native canvas) auto-scaled to fit any screen.
   - Full keyboard navigation (Arrow keys, Space, Fullscreen 'F', Overview Grid 'G', PDF print 'P').
   - High-contrast card containers with subtle box shadows.
   - High-quality inline SVG vector candlestick charts illustrating every technical concept.
   - Include an interactive challenge slide with toggle buttons to reveal answers step-by-step.
   - Include @media print stylesheet for 1-click clean export to PDF.
5. Educational Arc:
   - Follow the standard 18-19 slide structure: Cover -> Hook -> Agenda -> Disclaimer -> Core Value -> Detailed Concepts with SVG charts -> Comparison Tables -> Playbook -> Interactive Quiz -> Golden Rules -> 3 Pillars Integration (Strategy, Risk, Psychology) -> Q&A.

Please generate the complete, production-ready code (index.html, style.css, script.js) with no placeholders.
```

---

## 📂 5. Workspace Assets Reference

When referencing assets in your code:
- **Logo (Circular / Icon)**: `assets/logo.png` (or `../Asset/logo.png`)
- **Horizontal Banner Logo**: `assets/horizontal.png` (or `../Asset/horizontal.png`)
- **Sample Reference Deck**: `sample/AUPP Trading Club — Week 1 -  Fundamentals.pdf`
