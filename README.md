# PromptEasy

A barebones web teleprompter application for solo content creators. Scrolls text at configurable speeds with mirror mode support for beam-splitter rigs. Zero backend, fully client-side.

## Features

- **File Support**: Upload .txt, .docx, or .md files (up to 5MB)
- **Paste Text**: Paste text directly into the application
- **Auto-scroll**: WPM-based scrolling (60-300 WPM, default 180 WPM)
- **Mirror Mode**: Horizontal flip for beam-splitter teleprompter rigs
- **Font Control**: Adjustable font size (24-96px, default 48px)
- **Sentence Navigation**: Jump to previous/next sentence instantly
- **Progress Tracking**: Visual progress indicator showing percentage through document
- **Fullscreen Mode**: Distraction-free presentation
- **Persistent Settings**: Settings saved to browser localStorage
- **Keyboard Shortcuts**: Full keyboard control for hands-free operation

## Usage

### Getting Started

1. Open `index.html` in a modern web browser
2. Upload a file or paste your script text
3. Adjust speed and font size to your preference
4. Click play or press spacebar to start scrolling

### Keyboard Shortcuts

- **Spacebar**: Play/Pause
- **↑ Arrow**: Increase speed by 10 WPM
- **↓ Arrow**: Decrease speed by 10 WPM
- **← Arrow**: Previous sentence
- **→ Arrow**: Next sentence
- **F**: Toggle fullscreen

### Controls

#### Header Controls
- **Upload**: Load .txt, .docx, or .md files
- **Paste**: Open paste dialog for direct text input
- **Mirror**: Toggle horizontal flip for beam-splitter setups
- **Font**: Adjust text size (24-96px)
- **Speed**: Adjust scroll speed (60-300 WPM)
- **Fullscreen**: Enter/exit fullscreen mode

#### Footer Controls
- **◄**: Jump to previous sentence
- **▶/▐▐**: Play/Pause scrolling
- **►**: Jump to next sentence
- **Progress Bar**: Click to jump to specific position in document
- **Percentage**: Current progress through document

## Technical Details

- **Stack**: HTML5, CSS3, vanilla JavaScript
- **Dependencies**: mammoth.js (loaded via CDN for .docx parsing)
- **Storage**: localStorage for settings persistence
- **Browser Support**: Modern evergreen browsers (Chrome, Firefox, Safari, Edge)

## Acceptance Criteria

- ✅ Loads .txt, .docx, .md files under 5MB
- ✅ Smooth scroll at set WPM
- ✅ Settings persist across browser sessions
- ✅ Mirror mode accurately flips horizontal
- ✅ Sentence navigation with instant jumps
- ✅ Works offline (after initial load)
- ✅ Mobile responsive

## Hosting

Deploy to any static hosting service:

### GitHub Pages
1. Push code to GitHub repository
2. Go to Settings → Pages
3. Select branch and root folder
4. Save and wait for deployment

### Local Testing
Simply open `index.html` in your browser - no server required!

## Settings Persistence

The following settings are automatically saved to localStorage:
- `prompter_speed`: Scroll speed in WPM
- `prompter_fontSize`: Font size in pixels
- `prompter_mirror`: Mirror mode enabled/disabled

## Browser Compatibility

Requires a modern browser with support for:
- FileReader API
- Fullscreen API
- localStorage
- CSS transforms
- ES6 JavaScript

## License

Open source - feel free to use and modify for your needs.
