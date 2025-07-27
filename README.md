# Chat Compass 🧭

An app for viewing, searching, and analyzing your exported LLM chat conversations from ChatGPT and Claude.

**🌐 Live Demo:** [chat-compass.vercel.app](https://chat-compass.vercel.app/)  

[recording.webm](https://github.com/user-attachments/assets/d8636e59-854d-4d0d-a669-d730490e9d8d)

## 🚀 Features

### 📁 **Multi-Platform Support**
- **ChatGPT exports** - Import your conversation history from OpenAI
- **Claude exports** - View chats and projects from Anthropic's Claude
- **Multiple file formats** - Support for JSON files and ZIP archives
- **Batch processing** - Upload multiple files at once

### 🔍 **Advanced Search & Navigation**
- **Conversation search** - Find chats by title
- **Content search** - Search within message content with toggle option
- **Real-time filtering** - Instant results as you type
- **Smart highlighting** - Visual highlighting of search terms
- **Sorting options** - Sort by date (newest/oldest first)

### 💬 **Rich Message Display**
- **Formatted conversations** - Clean, readable chat interface
- **Syntax highlighting** - Code blocks with Prism.js highlighting for 60+ languages
- **Copy code buttons** - One-click copying of code snippets
- **Attachment support** - View file attachments and extracted content
- **Thinking process** - Expandable Claude reasoning sections
- **Message roles** - Clear visual distinction between user and assistant messages

### 🎨 **Modern Interface**
- **Dark/Light mode** - Toggle between themes with persistent preferences
- **Responsive design** - Works on desktop, tablet, and mobile
- **Collapsible sidebar** - Maximize reading space when needed
- **Smooth animations** - Polished user experience
- **Custom scrollbars** - Enhanced scrolling experience

### 📊 **Projects Tab** (Claude)
- **Project browser** - Navigate through Claude projects
- **Document viewer** - Read project documentation and files
- **Content search** - Find specific projects and documents
- **Metadata display** - Creation dates, descriptions, and details

### 🔗 **Integration Features**
- **Direct links** - Jump to original conversations on ChatGPT/Claude
- **Share functionality** - Copy chat links to clipboard
- **Scroll preferences** - Start at top or bottom of conversations
- **Chat counters** - Track total and filtered conversation counts

### 🔒 **Privacy & Security**
- **100% client-side processing** - All data stays in your browser
- **No server uploads** - Files are processed locally using JavaScript
- **No data transmission** - Your conversations never leave your device
- **Safe to use** - Can be run offline or on the hosted version

## 📥 Getting Your Data

### ChatGPT Export
1. Go to [ChatGPT Settings → Data Controls](https://chatgpt.com/#settings/DataControls)
2. Click "Export data"
3. Download the ZIP file when ready
4. Upload to Chat Compass

### Claude Export
1. Visit [Claude Settings → Data Privacy Controls](https://claude.ai/settings/data-privacy-controls)
2. Request data export
3. Download the provided files
4. Upload JSON files or ZIP archive to Chat Compass

## 🛠️ Installation & Usage

### Option 1: Use Hosted Version
Simply visit [chat-compass.vercel.app](https://chat-compass.vercel.app/) and start using it immediately.

### Option 2: Run Locally
1. Clone this repository
2. Open `index.html` in any modern web browser
3. No additional setup required!

### Getting Started
1. **Upload your data** - Drag and drop JSON/ZIP files or click to select
2. **Browse conversations** - Use the sidebar to navigate your chats
3. **Search and filter** - Find specific conversations or content
4. **Explore projects** - Switch to Projects tab for Claude project data
5. **Customize experience** - Toggle dark mode, collapse sidebar, adjust settings

## 🎯 Why Chat Compass?

I wanted a better way to view and search through my exported LLM conversations. I discovered [LLM Chat Explorer](https://github.com/levysoft/llm-chat-explorer) as a starting point and built additional features on top of it using Claude Code, including:

- Enhanced UI with dark mode and responsive design
- Advanced search capabilities with content filtering
- Code syntax highlighting with copy functionality
- Attachment and project support
- Improved conversation threading and display
- Modern styling and smooth user experience

## 💰 Development Cost
<img width="1622" height="513" alt="image" src="https://github.com/user-attachments/assets/18b5d507-10fe-4548-b7fe-9552b9d52df0" />

using: https://ccusage.com/

## 🏗️ Built With

- **Vanilla JavaScript** - No frameworks, pure web technologies
- **Tailwind CSS** - Utility-first styling
- **Prism.js** - Syntax highlighting for code blocks
- **JSZip** - ZIP file processing
- **Font Awesome** - Icons and UI elements

---

**Made with ❤️ using [Claude Code](https://claude.ai/code)**
