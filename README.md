# Window Management Web API - Center-to-Center Lines

A web application that visualizes connections between multiple browser windows by drawing lines from the center of each window to the centers of all other open windows.

## Features

- ðŸªŸ **Multi-Window Support**: Open multiple windows and see them all connected
- ðŸŽ¨ **Color-Coded Windows**: Each window gets a unique color for easy identification
- ðŸ“ **Real-Time Updates**: Lines update automatically when windows are moved or resized
- ðŸ”„ **Auto-Sync**: New windows automatically connect to existing ones
- ðŸ“± **Responsive**: Works across different window sizes and screen resolutions

## How It Works

The application uses the BroadcastChannel API to communicate between windows of the same origin. Each window:
- Calculates its center position in screen coordinates
- Broadcasts its position to other windows
- Draws lines connecting to all other open windows
- Updates in real-time as windows move or resize

## Usage

1. Open the page in your browser
2. Click "open another window" to create additional windows
3. Move or resize windows to see the connections update in real-time
4. Each window shows its own center point with a yellow dot

## Technical Details

- Uses HTML5 Canvas for drawing
- BroadcastChannel API for cross-window communication
- Screen coordinate system for accurate positioning
- Device pixel ratio support for high-DPI displays

## Live Demo

Visit the [GitHub Pages site](https://ezzcodeezzlife.github.io/window-connections/) to try it out!

## License

MIT License - feel free to use this code for your own projects.

