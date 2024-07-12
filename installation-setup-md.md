# Installation and Setup

Setting up the Cyberpunk Decryption project is straightforward. Follow these steps to get the project running on your local machine.

## Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Basic knowledge of using the command line (for cloning the repository)

## Installation Steps

1. **Clone the Repository**
   ```
   git clone https://github.com/yourusername/cyberpunk-decryption.git
   ```

2. **Navigate to the Project Directory**
   ```
   cd cyberpunk-decryption
   ```

3. **Open the Project**
   - Simply open the `index.html` file in your preferred web browser.

## Running Locally

Due to browser security restrictions, some features (like audio) may not work when opening the HTML files directly from the file system. To fully experience the project, you can use a local server:

1. **Using Python (Python 3)**
   ```
   python -m http.server 8000
   ```

2. **Using Node.js**
   First, install `http-server` globally:
   ```
   npm install -g http-server
   ```
   Then, in the project directory, run:
   ```
   http-server
   ```

3. Open your browser and navigate to `http://localhost:8000` (or the port specified by your chosen method).

## Troubleshooting

- If you encounter any issues with audio not playing, ensure you're using a local server as described above.
- Make sure your browser's autoplay settings allow for audio to play automatically.

For more detailed gameplay instructions, refer to the [Gameplay Guide](gameplay-guide.md).
