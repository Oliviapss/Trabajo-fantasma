---
description: Repository Information Overview
alwaysApply: true
---

# SCORIK Information

## Summary
SCORIK is a web application that converts audio files (MP3) to music sheets. It's designed for musicians who want to play their favorite songs using sheet music on their instruments. The project was created by four students from ORT school: Mia Dzwonik, Julia Barrera, Olivia Palomino, and Victoria Meinrath.

## Structure
The repository contains a simple web application with the following structure:
- Root directory: Contains the main HTML file and image assets
- `.vscode`: Contains VS Code configuration for development
- `img`: Directory for additional image assets (currently empty)

## Language & Runtime
**Language**: HTML, CSS (inline)
**Framework**: Bootstrap 5.3.3
**Additional Libraries**: AlpineJS 3.x (for reactivity)
**Development Environment**: Visual Studio Code with Live Server (port 5501)

## Features & Functionality
**Core Features**:
- Audio to sheet music conversion (MP3 to music notation)
- Sheet music library for saving converted scores
- Editor for adding expression marks
- Creator for building custom sheet music

**Technical Implementation**:
- Converts MP3 files to WAV format
- Uses Crepe library with Fourier transform for pitch and tempo detection
- Determines time signature, note types, and musical structure
- Organizes information in JSON format
- Generates visual sheet music using music21 and MuseScore 3
- Processing time: approximately 10 minutes per conversion

## User Interface
**Main Components**:
- Hero section with violin background and SCORIK branding
- Zigzag central design element
- Information sections explaining the application's purpose and functionality
- File upload interface for MP3 selection
- Responsive design using Bootstrap framework

## Usage
The application allows users to:
1. Select MP3 files through the file upload interface
2. Convert audio to sheet music notation
3. View and edit the generated sheet music
4. Save and organize sheet music in a library

## Development
**Development Server**:
```bash
# Using VS Code Live Server extension on port 5501
# Start server by right-clicking index.html and selecting "Open with Live Server"
```

**External Dependencies**:
- Bootstrap 5.3.3 (CSS and JS via CDN)
- AlpineJS 3.x (via CDN)
- Google Fonts (Inter font family)
- Backend processing requires Crepe, music21, and MuseScore 3 (not included in repository)