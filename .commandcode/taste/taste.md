# Coding Style
- Prefers self-contained, single-file code with no external dependencies (no external CSS files, no JavaScript, no frameworks, no libraries, no external image services). Confidence: 0.95
- Prefers internal CSS inside `<style>` tags rather than separate CSS files. Confidence: 0.95
- Favors CSS Grid for layout structures. Confidence: 0.7

# Design Aesthetics
- Values a minimalist, content-first design philosophy — explicitly states "do not over-design" and "do not add unnecessary UI", letting actual content be the primary focus. Confidence: 0.9
- Prefers monochromatic dark themes (black, charcoal, grey, white) and absolutely avoids pink, magenta, rose, purple, and colorful gradients. Confidence: 0.9
- Prefers subtle, restrained animations and effects (e.g., scale(1.03) hovers, subtle glassmorphism) rather than bold or distracting transitions. Confidence: 0.8
- Prefers clean system fonts over decorative or custom fonts (e.g., Inter, -apple-system, BlinkMacSystemFont, Segoe UI). Confidence: 0.8

# CSS Techniques
- Uses `object-fit: cover` as the standard approach for handling images of varying aspect ratios and dimensions gracefully without distortion. Confidence: 0.8
- Uses CSS `clamp()` for responsive typography sizing (e.g., `clamp(2.8rem, 6vw, 4rem)`). Confidence: 0.85
- Uses subtle radial gradients with very low white-transparent opacities (e.g., `rgba(255,255,255,0.05)`) for background depth rather than solid fills. Confidence: 0.8

# Glassmorphism
- Uses specific glassmorphism values: `rgba(255,255,255,0.05)` transparent white backgrounds for containers, `rgba(0,0,0,0.45)` for label overlays, `blur(12px)` for card containers, and `blur(8px)` for labels. Confidence: 0.85

# Workflow & Verification
- Inspects the project folder and reads files (README, directory listings) before writing code, to use actual filenames and paths rather than invented ones. Confidence: 0.9
- URL-encodes image filenames in `src` attributes when they contain spaces or special characters (e.g., `WhatsApp%20Image%202026-08-19.jpeg`). Confidence: 0.8
- Verifies file existence via system shell commands (e.g., `ls` or `for file in *.jpeg`) after creating the HTML, to confirm paths resolve correctly. Confidence: 0.8