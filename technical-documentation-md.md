# Technical Documentation

This document provides an overview of the technical aspects of the Cyberpunk Decryption project.

## Project Structure

```
cyberpunk-decryption/
│
├── index.html
├── data-stream.html
├── neural-network.html
├── README.md
├── css/
│   └── styles.css
├── js/
│   ├── main.js
│   ├── data-stream.js
│   └── neural-network.js
└── assets/
    ├── audio/
    │   ├── background-music.mp3
    │   ├── data-stream-sound.mp3
    │   └── node-activation-sound.mp3
    └── images/
        └── favicon.ico
```

## Technologies Used

- **HTML5**: Structure of the web pages
- **CSS3**: Styling and animations
- **JavaScript**: Core game logic and interactivity
- **Particles.js**: Background particle animations
- **Howler.js**: Audio management

## Key Components

### 1. Particle Background (index.html)

The main page uses Particles.js to create a dynamic background effect. The configuration for this can be found in the `<script>` tag at the bottom of `index.html`.

### 2. Data Stream Puzzle (data-stream.html)

The data stream puzzle uses JavaScript to:
- Generate random binary data
- Insert a hidden 4-digit code
- Animate the data stream
- Check user input against the hidden code

Key functions:
- `generateRandomData()`: Creates the binary stream with hidden code
- `createDataElement()`: Adds new data elements to the DOM
- `checkCode()`: Verifies user input

### 3. Neural Network Puzzle (neural-network.html)

The neural network visualization uses HTML5 Canvas and JavaScript to:
- Create a network of nodes and connections
- Handle user interactions (node activation)
- Check for correct activation sequence

Key classes:
- `Node`: Represents individual nodes in the network
- `Connection`: Represents connections between nodes

Key functions:
- `createNetwork()`: Initializes the neural network
- `animateNetwork()`: Renders the network on canvas
- `checkActivation()`: Verifies correct node activation

### 4. Audio Management

Howler.js is used for managing audio across the experience. Background music and sound effects are implemented in each HTML file using Howler.

## Performance Considerations

- The particle background and neural network animation can be resource-intensive. Consider optimizing or disabling these on lower-end devices.
- Audio files should be compressed appropriately to reduce load times.

## Browser Compatibility

The project is designed to work on modern browsers (Chrome, Firefox, Safari, Edge). Some features may not work correctly on older browsers or Internet Explorer.

## Future Enhancements

Potential areas for improvement:
- Implement a backend for user progress tracking
- Add more puzzles and expand the storyline
- Optimize performance for mobile devices
- Implement accessibility features (e.g., screen reader support)

For any technical questions or contributions, please refer to the [Contributing Guidelines](contributing.md).
