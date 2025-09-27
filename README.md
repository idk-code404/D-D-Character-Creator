D&D Character Creator
A responsive, user-friendly Dungeons & Dragons character creator that works directly in your browser. Create, customize, and save your D&D characters with ease!

https://img.shields.io/badge/D&D-5th%2520Edition-red https://img.shields.io/badge/GitHub-Pages-brightgreen https://img.shields.io/badge/License-MIT-blue

Features
🎭 Character Creation
Complete Character Sheet: Name, race, class, background, alignment, and ability scores

Real-time Preview: See your character sheet update as you make changes

Custom Options: Add your own custom races, classes, backgrounds, and alignments

Random Generation: Quickly create balanced random characters

💾 Data Management
Local Storage: Save characters directly in your browser

Character Management: Load, save, and delete multiple characters

Export Functionality: Export characters for printing or sharing

🎨 User Experience
Responsive Design: Works perfectly on desktop and mobile devices

D&D Themed UI: Authentic parchment-style design with appropriate colors

Tabbed Interface: Organized view of personality traits, ideals, bonds, and flaws

Custom Options Manager: Easy management of homebrew content

Quick Start
Option 1: Use on GitHub Pages
Visit the live version: https://yourusername.github.io/dnd-character-creator

Start creating characters immediately!

Option 2: Run Locally
Download the index.html file

Open it in any modern web browser

No server required - it works completely client-side!

How to Use
Basic Character Creation
Enter Character Details: Fill in name, race, class, background, and alignment

Set Ability Scores: Use the standard array or input custom values (1-20)

Add Personality: Describe traits, ideals, bonds, and flaws

Save Character: Click "Save Character" to store in your browser

Adding Custom Options
Enter Custom Content: Type your custom race, class, background, or alignment in the text field below the dropdown

Click Add: Press the "Add" button or hit Enter

Select from Dropdown: Your custom option will appear in the selection menu

Manage Options: Use the "Manage Custom Options" button to view or remove custom content

Managing Characters
Save: Stores your current character to browser storage

Load: Restore any previously saved character

Delete: Remove characters you no longer need

Random: Generate a balanced random character instantly

Technical Details
Browser Compatibility
Chrome 60+

Firefox 55+

Safari 12+

Edge 79+

Storage
All data is stored locally in your browser using:

localStorage: For character data and custom options

No server-side components: Complete privacy and offline functionality

File Structure
text
dnd-character-creator/
│
├── index.html          # Main application file
└── README.md           # This file
Customization
Adding New Default Options
Edit the index.html file and add new options to the appropriate <select> elements:

html
<select id="race">
    <option value="">Select a race</option>
    <option value="human">Human</option>
    <!-- Add new options here -->
    <option value="your-custom-race">Your Custom Race</option>
</select>
Modifying the Theme
Change CSS variables in the :root section to customize colors:

css
:root {
    --primary: #8B4513;    /* Main brown color */
    --secondary: #D2B48C;  /* Tan color */
    --accent: #CD853F;     /* accent color */
    /* ... more variables */
}
API Reference (For Developers)
The application uses a simple JavaScript API for character management:

Character Object Structure
javascript
{
    name: "Character Name",
    race: "human", // or "custom-YourRace"
    class: "wizard", // or "custom-YourClass"
    background: "sage", // or "custom-YourBackground"
    alignment: "lawful-good", // or "custom-YourAlignment"
    strength: 15,
    dexterity: 14,
    constitution: 13,
    intelligence: 12,
    wisdom: 10,
    charisma: 8,
    personality: "Personality description",
    ideals: "Character ideals",
    bonds: "Character bonds",
    flaws: "Character flaws"
}
Available Functions
saveCharacter() - Save current character to localStorage

loadCharacter(index) - Load character by index

deleteCharacter(index) - Delete character by index

generateRandomCharacter() - Create random character

addCustomOption(type, value) - Add custom option

removeCustomOption(type, value) - Remove custom option

Frequently Asked Questions
❓ How do I reset my characters?
Clear your browser's localStorage for this site, or use the delete function for individual characters.

❓ Can I use this for other RPG systems?
While designed for D&D 5e, the custom options make it adaptable for other systems with similar character structures.

❓ Is my data secure?
Yes! All data stays in your browser - nothing is sent to any server.

❓ Why can't I export to PDF?
The export function is a placeholder. For now, use your browser's print function (Ctrl+P) to save as PDF.

Contributing
Contributions are welcome! Here's how you can help:

Fork the repository

Create a feature branch (git checkout -b feature/amazing-feature)

Commit your changes (git commit -m 'Add amazing feature')

Push to the branch (git push origin feature/amazing-feature)

Open a Pull Request

Areas for Improvement
PDF export functionality

More detailed character sheets (skills, inventory, spells)

Character sharing features

Mobile app version

License
This project is licensed under the MIT License - see the LICENSE file for details.

Disclaimer
This tool is not affiliated with, endorsed, sponsored, or specifically approved by Wizards of the Coast LLC. This tool may use the trademarks and other intellectual property of Wizards of the Coast LLC, which is permitted under Wizards' Fan Site Policy. DUNGEONS & DRAGONS, D&D, Wizards of the Coast, Forgotten Realms, the dragon ampersand, Player’s Handbook, Monster Manual, Dungeon Master’s Guide, D&D Adventurers League, all other Wizards of the Coast product names, and their respective logos are trademarks of Wizards of the Coast in the USA and other countries.

Support
If you encounter any issues or have questions:

Check this README for answers

Examine the browser console for error messages

Create an issue in the GitHub repository
