# Tripod Pipeline

A web-based tool for AI-assisted Bible translation using the Tripod Method. This application orchestrates four AI agents through Google's Gemini API to create semantic meaning maps and generate natural oral translations.

## Overview

The Tripod Pipeline implements a four-agent workflow:

1. **Event Architect** (Agent 1): Creates structured Meaning Map JSON from biblical text
2. **Discourse Weaver** (Agent 2): Adds discourse structure and inter-event relations
3. **Oral Renderer** (Agent 3): Generates natural oral translation in the target language
4. **Accuracy Checker** (Agent 4): Validates faithfulness and provides quality analysis

## Features

- Single-page web application with no backend required
- Uses Google Gemini API for all AI processing
- Step-by-step workflow with manual review at each stage
- Copy/paste outputs between agents or use automatic "Pull from Previous" feature
- API key stored locally in browser (never sent to any server except Google)
- Clean, professional interface optimized for translation teams

## Quick Start

### Option 1: GitHub Pages (Recommended)

1. Fork this repository
2. Go to Settings → Pages
3. Select "Deploy from a branch" and choose `main` branch
4. Your app will be available at `https://[username].github.io/tripod-pipeline/`

### Option 2: Local Use

1. Download `index.html`
2. Open it directly in your web browser
3. No server required

## Usage

1. **Enter your Gemini API Key**
   - Get one free at [Google AI Studio](https://aistudio.google.com/apikey)
   - The key is stored locally in your browser

2. **Enter the Biblical Reference**
   - Example: `Ruth 1:1-5` or `Genesis 22:1-19`

3. **Set Target Language and Audience**
   - Example: Portuguese, Rural Brazil / Sertanejo

4. **Click "Start Pipeline"**
   - This opens Agent 1 with a prepared prompt

5. **Work through each agent:**
   - Review the input prompt
   - Click "Run Agent" to process
   - Review the output
   - Make edits if needed
   - Move to the next agent

## Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Google Gemini API key (free tier available)
- Internet connection

## Tripod Method

The Tripod Method is a semantic composition architecture for AI-assisted Bible translation. It separates meaning representation from linguistic expression using three components:

- **Meaning Maps**: Structured semantic representations using cognitive primitives
- **Language Archive**: Tagged authentic speech from the target community
- **Concept Bank**: Validated expressions for key biblical terms

Learn more: [Ready Vessels Project](https://www.shemaywam.com)

## Technical Details

- Pure HTML/CSS/JavaScript - no build step required
- **Model options:**
  - **Gemini 2.5 Pro** (recommended) - Best for complex linguistic analysis
  - **Gemini 2.5 Flash** - Good balance of quality and speed
  - **Gemini 2.0 Flash** - Fastest, for quick iterations
- Responsive design works on desktop and mobile
- All processing happens client-side

## File Structure

```
tripod-pipeline/
├── index.html      # Complete application (single file)
├── README.md       # This file
└── LICENSE         # MIT License
```

## License

MIT License - See [LICENSE](LICENSE) file

## Credits

- Tripod Method: Ready Vessels Project, OBT Lab, University of the Nations
- Contact: marcia.suzuki@uofn.edu

## Version

Tripod Pipeline v5.2 | January 2026
