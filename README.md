# 🧠 SRS Memorizer

A modern, browser-based Spaced Repetition System (SRS) application for efficient memorization. Inspired by Anki, but built with simplicity and modern web technologies in mind.

## 🌟 Features

### Core SRS Functionality
- **Smart Algorithm**: Simplified SM-2 algorithm for optimal review intervals
- **Intuitive Review**: Four-level difficulty rating (Again, Hard, Good, Easy)
- **Progress Tracking**: Visual statistics and learning metrics
- **Deck Management**: Create, edit, and organize cards into thematic decks
- **Tagging System**: Organize content with custom tags

### Import/Export Capabilities
- **Full Backup/Restore**: Export all data as JSON for backup
- **Single Deck Export**: Share individual decks with others
- **Anki Compatibility**: Export decks to CSV format for use in Anki
- **Smart Import**: Import decks with options to preserve progress or merge data
- **Data Validation**: Safe import with format validation and error reporting

### User Experience
- **SPA Architecture**: Single-page application with smooth navigation
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Offline First**: All data stored locally in your browser
- **Clean UI**: Modern interface built with Bootstrap and Font Awesome
- **Progress Visualization**: Charts and stats to track learning progress

## 🚀 Quick Start

1. **Clone or Download**: Simply download the `index.html` file
2. **Open in Browser**: Double-click `index.html` to launch the application
3. **Start Learning**: No installation required - everything runs in your browser!

## 📁 File Structure

```
srs-memorizer/
├── index.html          # Main application file (everything included)
└── README.md           # This documentation
```

## 🎮 How to Use

### Creating Content
1. **Create a Deck**: Click "New Deck" and give it a name and description
2. **Add Cards**: Open a deck and click "Add Card"
3. **Tag Your Cards**: Use tags for better organization

### Learning Process
1. **Start Review**: Click "Start Review" on any deck with due cards
2. **View Question**: Try to recall the answer
3. **Reveal Answer**: Click "Show Answer" when ready
4. **Rate Difficulty**: Select how well you remembered (Again/Hard/Good/Easy)
5. **Continue**: The system will show the next card automatically

### Managing Data
- **Export Deck**: Click the menu (⋮) on any deck → "Export"
- **Import Deck**: Use the import option in the navigation menu
- **Full Backup**: Go to Statistics → "Export All Data"
- **Restore Backup**: Statistics → "Import Backup"
- **Export to Anki**: Deck card menu → "Export to Anki"

## 🔧 Technology Stack

- **Frontend**: Alpine.js (Reactive JavaScript framework)
- **UI Framework**: Bootstrap 5 (Responsive design)
- **Icons**: Font Awesome 6
- **Fonts**: Google Fonts (Inter, Roboto Mono)
- **Storage**: Browser LocalStorage
- **Format**: Single-file SPA (no build process required)

## 📊 SRS Algorithm Details

The application uses a simplified SM-2 algorithm:

### Interval Calculation
- **First review**: 1, 3, 7, or 16 days based on difficulty rating
- **Subsequent reviews**: Previous interval × ease factor
- **Ease factor**: Adjusts based on performance (1.3-2.5 range)

### Difficulty Ratings
- **Again (0)**: Reset interval, decrease ease factor
- **Hard (1)**: Small interval increase
- **Good (2)**: Normal interval increase, slight ease factor increase
- **Easy (3)**: Larger interval increase, ease factor increase

## 🗂️ Data Formats

### SRS Memorizer JSON Format
```json
{
  "formatVersion": "1.0",
  "appName": "SRS Memorizer",
  "exportType": "single_deck",
  "exportedAt": "2024-01-15T10:30:00Z",
  "data": {
    "deck": { ... },
    "cards": [ ... ]
  }
}
```

### Anki-Compatible CSV Format
```
Front;Back;Tags
"Question 1";"Answer 1";"tag1 tag2"
"Question 2";"Answer 2";"tag3"
```

## 🚀 Deployment Options

### Option 1: Local Use
- Simply open `index.html` in any modern browser
- Works offline after initial load

### Option 2: Web Hosting
- Upload `index.html` to any static hosting service:
  - GitHub Pages
  - Netlify
  - Vercel
  - Cloudflare Pages
  - Any traditional web host

### Option 3: Self-Hosted
- Place the file on any web server
- Access via `http://your-domain.com/path/to/index.html`

## 📱 Browser Compatibility

- Chrome 90+ ✅
- Firefox 88+ ✅
- Safari 14+ ✅
- Edge 90+ ✅
- Mobile browsers ✅

## 🔒 Data Privacy

- **100% Local**: All data stays in your browser
- **No Tracking**: No analytics, no external calls
- **No Server**: No data leaves your device
- **Backup Control**: You control when and where to backup data

## 🛠️ Development

### No Build Required
This is a single HTML file with inline CSS and JavaScript - no build tools needed!

### Customization Options
1. **Styles**: Edit the `<style>` section in the HTML
2. **Functionality**: Modify the Alpine.js code in the `<script>` tags
3. **Icons**: Replace Font Awesome with other icon sets
4. **Theming**: Customize Bootstrap variables or replace with another CSS framework

### Extending the Application
- Add audio support using the Web Audio API
- Implement image upload with canvas compression
- Add collaborative features with WebRTC
- Create PWA capabilities with a service worker
- Add dark/light theme toggle

## 🤝 Contributing

While this is a single-file application, you can:
1. Fork the repository
2. Make improvements to the HTML/CSS/JS
3. Submit a pull request
4. Or simply customize your own version!

## 📄 License

MIT License - feel free to use, modify, and distribute as needed.

## 🙏 Acknowledgements

- Inspired by **Anki** and **SuperMemo** spaced repetition systems
- Built with **Alpine.js** for reactive functionality
- Styled with **Bootstrap** for responsive design
- Icons by **Font Awesome**
- Fonts by **Google Fonts**

## 🐛 Issues & Feedback

Found a bug or have a feature request?
1. Check if it's already reported
2. Provide detailed steps to reproduce
3. Suggest your expected behavior

## 🌐 Live Demo

[Demo](https://pwrmind.github.io/SRSMemorizer/)

---

**Happy Learning!** 🎓

*Remember: Consistency beats intensity when it comes to spaced repetition.*
