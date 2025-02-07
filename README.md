# Battle Plan - Initiative Tracker

## Description

Battle Plan is a React-based initiative tracker designed to help Dungeon Masters and players manage combat encounters in Dungeons and Dragons and other tabletop role-playing games. It provides a simple and intuitive interface for tracking combatants, their initiative scores, status effects, and other relevant information. This application aims to streamline combat management, allowing for a more immersive and enjoyable gaming experience.

## Features

-   **Combatant Management:** Add, remove, and manage combatants (players, monsters, NPCs) with ease. Each combatant can be customized with a name, type, and initiative score.
-   **Initiative Tracking:** Enter and display initiative scores for each combatant. The application automatically sorts combatants by initiative to determine turn order.
-   **Turn Order Visualization:** Clearly displays the current turn order, highlighting the active combatant. A "Next Turn" button advances the turn, cycling through the combatants in the correct order.
-   **Status Effects:** Add and track status effects (e.g., poisoned, stunned, blessed) for each combatant. Status effects can have durations, and the application can automatically remove effects when their duration expires.
-   **Customizable Combatant Types:** Define custom combatant types (e.g., Player, Monster, NPC) with associated colors for easy visual identification.
-   **Round Counter:** Tracks the current round of combat.
-   **Responsive Design:** The application is designed to work well on various screen sizes, from desktop computers to mobile devices.
-   **PWA Support:** Installable as a Progressive Web App for offline use. This allows you to use the application even without an internet connection.
-   **Local Storage:** Combat data is stored in the browser's local storage, so your combat encounters are preserved even after closing the browser.
-   **Clear All:** Clear all combatants with a single click.

## Technologies Used

-   **React:** A JavaScript library for building user interfaces.
-   **styled-components:** A CSS-in-JS library for styling React components.
-   **lodash.clonedeep:** A utility library for deep cloning JavaScript objects.
-   **Workbox:** A library for creating Progressive Web Apps.

## Installation

1.  Clone the repository:

    git clone <repository-url>

2.  Navigate to the project directory:

    cd <project-directory>

3.  Install dependencies:

    npm install

## Usage

1.  Start the development server:

    npm start

2.  Open your browser and navigate to `http://localhost:3000`.

## Building for Production

1.  Build the project:

    npm run build

2.  The production-ready files will be in the `build` directory.

## PWA Features

This application is a Progressive Web App (PWA). It can be installed on your device for offline use.

*   **Service Worker:** A service worker is registered to cache assets and provide offline functionality. See `public/service-worker.js` for details.
*   **Manifest:** The `public/manifest.json` file provides metadata about the app, such as its name, icons, and display properties.

## Contexts

*   `CombatantContext` (src/Contexts/CombatantContext.jsx): Manages the state and functions related to combatants, such as adding, removing, and updating combatants. This context provides the core data and logic for the application.
*   `DropDownContext` (src/Contexts/DropDownContext.jsx): Manages the state of dropdown menus for editing combatant details. This context ensures that dropdown menus function correctly and consistently throughout the application.
*   `ModalContext` (src/Contexts/ModalContext.jsx): Manages the state and functions related to the modal, such as opening and closing the modal. This context provides a centralized way to control the modal's behavior.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues to suggest improvements or report bugs.