# Crisis Room Brasil 2026

## Project Overview
**Crisis Room Brasil 2026** is a browser-based geopolitical decision simulator. It gamifies the "Top Risks 2026" report by the Eurasia Group, allowing players to navigate complex scenarios from a Brazilian perspective (or US perspective in the legacy version).

The application is a self-contained static web page, designed for zero-setup execution.

## Key Files

*   **`game_brasil.html`**: The primary application file. Contains the game engine, UI, and bilingual content (PT/EN). This is the file to edit for new features or content updates.
*   **`game.html`**: The original English-only version, focused on a US perspective. Kept for reference.
*   **`software_ideas.md`**: Design document outlining the origin of the project and other potential software ideas based on the source report.
*   **`README.md`**: User-facing documentation.

## Architecture & Technology
*   **Type:** Static Web Application (Single Page).
*   **Stack:** Vanilla HTML5, CSS3, and JavaScript.
*   **Structure:** All resources (styles, scripts, game data) are embedded directly within the HTML files to ensure portability.
    *   **CSS:** Located in the `<head>` style block.
    *   **Logic:** Located in `<script>` tags at the bottom of the body.
    *   **Content:** Hardcoded JavaScript objects/arrays usually represent scenarios and game states.

## Development & Usage

### Running the Project
There is no build server or installation required.
1.  Navigate to the project directory.
2.  Open `game_brasil.html` in any modern web browser (Chrome, Firefox, Edge).

### editing Guidelines
*   **Single-File Logic:** When making changes, ensure you are editing the correct section (CSS vs HTML vs JS) within `game_brasil.html`.
*   **Bilingual Support:** New content must be added for both Portuguese (`pt`) and English (`en`) in the data structures to maintain the language toggle functionality.
*   **Visual Style:** The design uses a dark, "situation room" aesthetic with gradients (#0a1628 to #0a2e1f). Maintain this visual consistency.
