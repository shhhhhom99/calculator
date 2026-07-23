

Thermal Precision Scale Converter

A clean, modern, and highly precise web-based temperature conversion utility developed as a collegiate engineering/web development project. The application allows users to seamlessly convert temperatures between Celsius, Fahrenheit, and Kelvin scales, while tracking history and viewing dynamic scale benchmarks.

 Features

Tri-Scale Conversion: Supports precise transformations between Celsius (°C), Fahrenheit (°F), and Kelvin (K).
Dynamic Scale Benchmarks: Displays critical references instantly (Absolute Zero, Freezing point, Room Temperature, Body Temperature, and Boiling point) which adapt based on the selected scale.
Thermal Zone Analytics: Provides semantic contextual descriptions (e.g., Sub-Zero Freezing) based on the current calculated thermal thresholds.
Calibration History Log: A persistent sidebar logging system that records conversion values, timestamps, and custom process notes for quality control tracking.
Quick Presets: One-click automated inputs for standard scientific reference points.
Modern UI Engine: Supports Dark Mode toggle, clean responsive typography, and an industrial-grid dashboard aesthetic.

---

 Mathematical Formulas Applied

The core conversion engine operates using standard thermodynamic conversions:

From Celsius (°C)
Fahrenheit:
$[°F] = [°C] \times \frac{9}{5} + 32$
Kelvin:
$[K] = [°C] + 273.15$

From Fahrenheit (°F)
Celsius:
$[°C] = ([°F] - 32) \times \frac{5}{9}$
Kelvin:
$[K] = ([°F] - 32) \times \frac{5}{9} + 273.15$

From Kelvin (K)
Celsius:
$[°C] = [K] - 273.15$
Fahrenheit:
$[°F] = ([K] - 273.15) \times \frac{9}{5} + 32$

---

Technology Stack

HTML5: Semantic architecture for layout configuration and data inputs.
CSS3: Custom layout system with responsive breakpoints, grid alignments, and dynamic styling variables for theme toggles.
JavaScript (ES6+): Pure vanilla JS logic managing state transformations, string formatting mathematical precisions, and DOM modifications.

