# D&D Style Text Adventure Game

## Overview

This project is a simple, browser-based text adventure game inspired by Dungeons & Dragons (D&D). It features a choice-based narrative with dice rolling mechanics for skill checks and combat scenarios. The game is built using HTML, CSS, and JavaScript, making it easy to host on platforms like GitHub Pages.

## Features

- Text-based adventure gameplay
- D&D-inspired dice rolling mechanics
- Simple inventory and stat tracking
- Branching narrative based on player choices
- Easy to customize and expand

## Live Demo

You can play the game here: [Your GitHub Pages URL]

## Setup

To set up this game on your own GitHub Pages:

1. Fork this repository to your GitHub account.
2. Clone the forked repository to your local machine.
3. Ensure the main HTML file is named `index.html`.
4. Push your changes to GitHub.
5. Go to your repository settings on GitHub.
6. Scroll down to the GitHub Pages section.
7. Set the source to the main branch and save.

Your game should now be live at `https://[your-username].github.io/[repository-name]/`.

## Customization

### Adding New Scenes

To add new scenes to the game:

1. Open `index.html` in a text editor.
2. Locate the `scenes` object in the JavaScript section.
3. Add a new scene following this template:

```javascript
yourNewScene: {
    text: "Description of the scene",
    choices: [
        { text: "Choice 1", nextScene: "sceneForChoice1" },
        { text: "Choice 2", nextScene: "sceneForChoice2" }
    ],
    effect: () => {
        // Optional: Add any effects that should occur when entering this scene
    }
}
```

4. Link your new scene from existing scenes by updating their `nextScene` properties.

### Modifying Game Mechanics

- To change dice rolling mechanics, modify the `rollDice` function.
- To alter character stats, update the variables at the top of the script (e.g., `playerHealth`, `playerStrength`).
- To change how dice rolls affect gameplay, modify the `effect` functions in relevant scenes.

## Contributing

Contributions to improve the game are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Inspired by Dungeons & Dragons and classic text adventure games.
- Built with vanilla JavaScript, HTML, and CSS.

## Contact

[Your Name] - [Your Email/Contact Information]

Project Link: [https://github.com/your-username/your-repo-name](https://github.com/your-username/your-repo-name)
