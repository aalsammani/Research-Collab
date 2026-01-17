# ResearchSync — Collaborative Research Document Editor

<div align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License">
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome">
</div>

<p align="center">
  <strong>A modern, collaborative document editor for researchers</strong><br>
  Write LaTeX papers and Word documents together in real-time
</p>

---

## ✨ Features

### 📝 Dual Editor Modes
- **LaTeX Editor** — Full-featured TeX editor with live preview, syntax highlighting, and math rendering via KaTeX
- **Word Editor** — Rich text editing with familiar formatting tools

### 👥 Real-Time Collaboration
- See collaborators' presence indicators
- Team chat for quick communication
- Comment system with threading and resolution
- Version history tracking

### 🛠️ Professional Tools
- **LaTeX Toolbar** — Quick insertion for sections, math, figures, tables, citations
- **Word Toolbar** — Bold, italic, headings, lists, alignment, and more
- **File Management** — Multi-file project support with folder organization
- **Export Options** — Export to `.tex`, `.docx`, `.pdf`, `.html`, `.md`

### 🎨 Modern Interface
- Clean, academic aesthetic designed for focus
- Dark/Light theme support
- Responsive layout
- Keyboard shortcuts

## 🚀 Quick Start

### Option 1: GitHub Pages
1. Fork this repository
2. Go to **Settings** → **Pages**
3. Select `main` branch and `/` (root) folder
4. Your site will be live at `https://yourusername.github.io/repository-name`

### Option 2: Local Development
```bash
# Clone the repository
git clone https://github.com/yourusername/research-collab.git

# Navigate to the directory
cd research-collab

# Open in browser (or use a local server)
open index.html
```

### Option 3: Deploy to Vercel/Netlify
Simply connect your GitHub repository and deploy automatically.

## 📖 Usage Guide

### LaTeX Editor

The LaTeX editor provides live preview with KaTeX math rendering:

```latex
\begin{equation}
    E = mc^2 + \sum_{i=1}^{n} \alpha_i x_i
\end{equation}
```

**Keyboard Shortcuts:**
- `Ctrl/Cmd + B` — Bold text
- `Ctrl/Cmd + I` — Italic text
- `Ctrl/Cmd + S` — Save document

**Toolbar Features:**
- Text formatting (bold, italic, underline)
- Sections and headings
- Math symbols and equations
- Lists (bullet and numbered)
- Citations and references
- Figures and tables

### Word Editor

The Word editor provides familiar rich-text editing:

- Format text with the toolbar
- Create headings and paragraphs
- Add bullet and numbered lists
- Align text (left, center, right, justify)
- Insert links

### Collaboration

1. **Invite Collaborators** — Click "Share" to invite team members
2. **Chat** — Use the chat panel for quick discussions
3. **Comments** — Add comments on specific text selections
4. **Version History** — Track all changes with timestamps

## 🗂️ Project Structure

```
research-collab/
├── index.html      # Main application file
├── README.md       # This file
└── LICENSE         # MIT License
```

## 🔧 Customization

### Themes

Toggle dark mode using the sun/moon icon in the header. Custom themes can be added by modifying the CSS variables:

```css
:root {
    --bg-primary: #faf9f7;
    --accent-primary: #2563eb;
    /* ... more variables */
}

[data-theme="dark"] {
    --bg-primary: #121212;
    /* ... dark theme overrides */
}
```

### Adding Features

The application is built with vanilla JavaScript for easy customization. Key areas:

- **Editor functionality**: `insertLatex()`, `formatWord()`
- **File management**: `state.files` object
- **Collaboration**: `state.collaborators`, `sendChatMessage()`
- **Export**: `exportDocument()`, `exportToDocx()`

## 📦 Dependencies

All dependencies are loaded via CDN:

- [KaTeX](https://katex.org/) — Math rendering
- [Mammoth.js](https://github.com/mwilliamson/mammoth.js) — Word document import
- [docx](https://github.com/dolanmiu/docx) — Word document export
- [Google Fonts](https://fonts.google.com/) — Crimson Pro, DM Sans, JetBrains Mono

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📋 Roadmap

- [ ] Real-time collaboration via WebRTC/WebSocket
- [ ] Cloud storage integration (Google Drive, Dropbox)
- [ ] PDF compilation service
- [ ] Bibliography management
- [ ] Overleaf import/export
- [ ] Mobile app

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by [Overleaf](https://overleaf.com/) and [Google Docs](https://docs.google.com/)
- Built with modern web technologies
- Designed for the academic community

---

<p align="center">
  Made with ❤️ for researchers everywhere
</p>
