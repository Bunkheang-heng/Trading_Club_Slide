# AUPP Trading Club Presentation Standard

This rule automatically applies whenever creating, modifying, or reviewing presentation slides in the `Trading_Club_Slide` workspace.

## Brand Identity & Visual Tokens
- **Theme**: Institutional finance, high aesthetic clarity, Wall Street & academic presentation standard.
- **Palette**:
  - Primary Navy: `#0D1F3C` / `#102A43`
  - Secondary Navy: `#16284F`
  - Accent Crimson: `#C8102E`
  - Bullish Green: `#00A868`
  - Bearish Red: `#E53E3E`
  - Background: `#FFFFFF` (Slide canvas), `#F8FAFC` (Cards)
  - Borders: `#E2E8F0`
- **Typography**:
  - Headings: `Cinzel` (Google Fonts, serif, letter-spacing: 0.03em)
  - Body & Badges: `Montserrat` (Google Fonts, sans-serif)
- **Signature Elements**:
  - Crimson underline bar (`width: 70px; height: 4px; background: #C8102E; border-radius: 2px; margin-top: 12px; margin-bottom: 24px;`) directly beneath every slide title.
  - Top-right header logo: `horizontal.png` from `assets/` or `Asset/`.
  - Cover and closing logo: `logo.png`.
  - Slide footer: `AUPP Trading Club • [Topic]` on left, topic name and 2-digit slide number badge on right.

## Technical Requirements for Web Slides
- **Aspect Ratio**: 16:9 widescreen canvas (`1440px x 810px` native) with responsive CSS transform/scale to fit any screen.
- **Keyboard Navigation**: Arrows, Space, PageUp/PageDown, 'F' for fullscreen, 'G' for slide overview modal, 'P' for print.
- **Visuals (Candlesticks + Line Graph)**:
  - Technical charts MUST display **BOTH Japanese candlesticks** (green/red bodies with wicks) **AND the structural line graph** overlaying the swing points.
  - Include view toggle buttons (`Both`, `Candlesticks`, `Line Only`) with "Both" active by default.
- **Interactive Features**: Include an interactive class practice/quiz slide with toggleable reveal buttons.
- **Print / PDF**: Include `@media print` stylesheet formatted for 16:9 landscape export with 0 margin.

## Curriculum Structure Standard (12–14 slides max)
- Keep lessons beginner-friendly, clean, intuitive, and easy to teach to university students.
- Avoid overcomplicating with advanced institutional concepts unless explicitly requested.

Standard Arc:
1. Cover (AUPP logo badge, title, subtitle, organized by & supported by credits)
2. Introduction & Simple Concept definition
3. Table of Contents (6 numbered cards)
4. Club Disclaimer (Risk management and educational acknowledgment)
5. The 3 Market Trends (Uptrend, Downtrend, Sideways)
6. Key Definitions / Abbreviations (HH, HL, LH, LL)
7. Uptrend (HH + HL anatomy & simple wave chart)
8. Downtrend (LH + LL anatomy & simple wave chart)
9. Sideways Market (Equal Highs & Equal Lows - Support & Resistance)
10. Break of Structure (BOS continuation)
11. Market Structure Shift (MSS reversal)
12. Quick Practice / Quiz (Clickable reveal buttons for class interaction)
13. Summary Key Takeaways & Q&A
