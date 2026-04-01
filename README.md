ChromaType | Palette & Font Generator

ChromaType is a lightning-fast, production-ready static web application that generates mathematically sound color palettes and curated Google Font pairings on demand. Built specifically for solo founders, developers, and indie hackers, it provides instant branding references within a visually sharp, frictionless UI.

✨ Features

Mathematically Sound Palettes: Generates colors using HSL cylindrical coordinate mapping. It locks a base hue and derives complementary (+180°) and triadic (+120°/240°) variants, completely avoiding the mud of purely random HEX generation.

Auto-Accessibility: Automatically calculates relative luminance and enforces a strict minimum WCAG contrast ratio of 4.5:1 between text and background colors via programmatic lightness adjustments.

Live Visual Preview: Every generated color and font instantly applies to a dynamic, interactive preview canvas featuring a hero section, typography scale, UI components, and interpolated gradients.

Granular Controls: Interactive Hue and Saturation sliders allow you to manipulate the mathematical base of your palette in real-time.

Lock & Roll: Found a primary color or font you like? Lock individual swatches or typography choices while randomizing the rest of the canvas.

Favorites System: Save your best generations directly to your browser's local storage.

Developer-Ready Exports: - One-click copy for individual HEX codes.

Instantly copy the entire palette and typography setup as :root CSS variables.

Export the current configuration as a structured .json file.

⌨️ Keyboard Shortcuts

Speed up your workflow without touching your mouse:

Space : Generate a new random palette and font pairing.

S : Save the current configuration to your Favorites.

C : Copy the entire palette to your clipboard as CSS variables.

🛠 Tech Stack

ChromaType is a masterclass in minimalism. It is designed to be fully self-contained with zero dependencies.

100% Vanilla: Pure HTML, CSS, and JavaScript.

Zero Build Steps: No Webpack, no Vite, no Node.js required.

Single-File Architecture: All logic, styling, state management, and SVG iconography live inside a single index.html file.

External Resources: Only utilizes the static Google Fonts API for typography rendering.

🚀 Getting Started

Because it requires no build tools or external assets, getting started takes less than a second:

Download or clone the repository.

Double-click index.html to open it in any modern web browser.

Press Spacebar to start generating!

🧠 Color Theory Math

The color generation relies on HSL (Hue, Saturation, Lightness) math. A base hue is established randomly (or by sliding the Hue control). The Primary color uses this exact hue, the Secondary color grabs its direct complement (+180°), and the Accent color is assigned a triadic variant (+120° or 240°).

The contrast engine converts HEX to linear RGB to determine relative luminance, tweaking lightness properties in 5% increments until all text elements comfortably pass web accessibility standards against their dynamic backgrounds.