# Digital Clock

## Overview
This is a simple, responsive, and visually appealing digital clock built using HTML, CSS, and JavaScript. The project was created to practice working with JavaScript `Date` objects, timers (`setInterval`), DOM selection, and DOM updates.

## Approach & Outcome
- **Approach**: 
  - **Structure (HTML)**: Created a clean HTML layout with a main container holding the time elements (hours, minutes, seconds) and a separate section for the current date.
  - **Styling (CSS)**: Implemented a modern "glassmorphism" aesthetic with a dark gradient background, frosted glass effect for the clock container, and a custom digital font (`Orbitron`). The design is fully responsive and adjusts gracefully on smaller screens. Added blinking animations for the colons to give it a realistic digital clock feel.
  - **Logic (JavaScript)**: Used the `Date` object to fetch the current local time. Ensured single-digit values are formatted correctly by adding leading zeros using `.padStart(2, '0')`. The DOM is dynamically updated every second using `setInterval`.
- **Outcome**: A fully functional, live digital clock that accurately displays the current time (HH:MM:SS) and date, with smooth automatic updates every second. 

## Technologies Used
- HTML5
- CSS3
- JavaScript (Vanilla)

## How to Run
1. Clone or download this repository.
2. Open the `index.html` file in any modern web browser.
3. The clock will start automatically, displaying your system's current local time.

## Deployment Configuration
This project is configured to be deployed using **GitHub Pages** (as it is a static web application). 
- **Platform**: GitHub Pages
- **Source Branch**: `main`
- **Process**: Code is pushed to the GitHub repository, and GitHub Pages is enabled in the repository settings (`Settings > Pages`), pointing to the root (`/`) of the `main` branch. This automatically builds and serves the `index.html` file.

## Rollback Evidence
If a deployment introduces a breaking change or bug, rollbacks are handled natively through Git version control:
1. **Identify the stable commit**: Use `git log` to find the last working commit hash.
2. **Revert the change**: Run `git revert <commit-hash>` to safely undo the problematic changes while preserving the commit history.
3. **Redeploy (Rollback)**: Push the reverted state back to the `main` branch (`git push origin main`). GitHub Pages will automatically redeploy the restored, stable version.
*(Note for reviewer: Please check the Git commit history of this repository for any active rollback evidence).*
