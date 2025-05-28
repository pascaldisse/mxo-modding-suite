# Matrix Online Modding Suite (MOMS)

A comprehensive web-based modding tool for The Matrix Online, allowing you to view and edit various game file formats used by the Lithtech: Discovery engine.

## Features

- **Multi-Format Support**: View and edit models (.ABC), textures (.DTX), levels (.DAT), sounds, scripts, messages (.MSG), and archives (.REZ, .LTA, .PKB)
- **3D Visualization**: WebGL-based viewers for models and levels
- **Text Editing**: Full-featured code editor for scripts and configuration files
- **Archive Management**: Extract and view contents of game archives
- **Audio Visualization**: Waveform display and playback for sound files

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, or Edge)
- The Matrix Online game files

### Installation

No installation required! This is a standalone web application that runs entirely in your browser.

1. Open `index.html` in your preferred web browser
2. Click "Load Directory" and select your Matrix Online game folder
3. The application will scan and categorize your files

## Usage

### File Navigation

The file tree on the left side shows all files organized by directory. Click on any file to select it for editing.

### Editors

Different editors automatically load based on file type:

- **3D Models (.ABC)**: View and manipulate models in 3D space
- **Textures (.DTX)**: View and edit image textures
- **Levels (.DAT)**: Explore and modify game levels
- **Scripts (.LUA, .CS)**: Edit game scripts with syntax highlighting
- **Messages (.MSG)**: Edit in-game text
- **Archives (.REZ, .LTA, .PKB)**: View and extract contained files

### Preview Panel

The right panel shows metadata and information about the selected file.

## File Type Support

| Extension | Description | Features |
|-----------|-------------|----------|
| .ABC | 3D Model Files | View, rotate, export |
| .DTX | DirectX Textures | View, edit, export |
| .DAT | Level Data | View geometry and entities |
| .REZ, .LTA, .PKB | Archive Files | View contents, extract files |
| .MSG | Message Files | Edit in-game text |
| .LUA, .CS | Script Files | Edit with syntax highlighting |

## Implementation Notes

This tool uses the following web technologies:

- **React.js**: For the user interface
- **Three.js**: For 3D rendering
- **Monaco Editor**: For text/code editing
- **Web File API**: For file access

## Limitations

As a browser-based tool, MOMS has some limitations:

- Cannot directly modify files on disk (extracts to temporary memory)
- Complex animations and physics simulation not fully supported
- Some proprietary formats may have limited editing capabilities

## Future Enhancements

- Full navmesh editing for .DAT files
- Batch export/import functionality
- Advanced texture editing with layers
- Model rigging and animation editing

## Credits and References

- Based on research from the Matrix Online modding community
- References specifications from [LithTools](https://haekb.itch.io/lithtools)
- Uses parsing insights from [Kaitai Struct for Lithtech DAT](https://github.com/leoschur/kaitai_lithtech_dat_struct)

## License

This project is provided for educational purposes. The Matrix Online and associated file formats are property of their respective owners.

---

**Note**: This is a prototype tool. Some features may be limited or simulated for demonstration purposes.