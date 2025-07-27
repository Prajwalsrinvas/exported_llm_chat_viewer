# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file web application called "LLM Chat Explorer" that provides a viewer for exported conversation data from ChatGPT and Claude. The entire application is contained in `llm-chat-explorer.html` - a standalone HTML file with embedded CSS and JavaScript.

## Architecture

### Core Components

- **Single HTML File**: The entire application is self-contained in one file with no external dependencies except CDN libraries
- **Frontend-only**: Pure client-side JavaScript application with no backend requirements
- **File Processing**: Handles both JSON and ZIP file uploads containing conversation exports
- **Data Formats**: Supports both ChatGPT (mapping-based) and Claude (chat_messages-based) export formats

### Key Functional Areas

1. **File Upload System** (lines 714-825)
   - Drag & drop interface
   - Supports multiple file types (.json, .zip)
   - Progress bar for large file processing

2. **Data Processing Engine** (lines 837-1131)
   - `processData()`: Main function that normalizes different export formats
   - `processZipFile()`: Handles ZIP file extraction using JSZip
   - Format detection and conversion between ChatGPT and Claude structures

3. **UI Components**
   - **Sidebar**: Chat list with search functionality and tabs for conversations/projects
   - **Main Content**: Message display area with formatted content
   - **Settings Modal**: Dark mode and chat positioning preferences

4. **Search System** (lines 941-1010)
   - Title-based search (default)
   - Optional content-based search within messages
   - Real-time filtering with highlighting

5. **Message Rendering** (lines 1038-1126)
   - Role-based styling (user vs assistant messages)
   - Thinking content support for Claude messages (collapsible sections)
   - Link detection and code block formatting

### Data Structure Handling

- **ChatGPT Format**: Uses `mapping` object with nested message structure
- **Claude Format**: Uses `chat_messages` array with direct message objects
- **Projects**: Separate handling for Claude projects with documents and prompt templates

## Development Notes

- No build process required - edit the HTML file directly
- All styles are embedded in `<style>` tags (lines 10-705)
- JavaScript is embedded in `<script>` tags (lines 826-1477)
- Uses Font Awesome CDN for icons and JSZip CDN for ZIP file processing
- Responsive design with mobile support
- Dark mode support with CSS custom properties
- LocalStorage used for user preferences (dark mode, chat positioning)

## Key Features

- Dual format support (ChatGPT and Claude exports)
- ZIP file support for batch imports
- Search with content filtering
- External link generation to original chats
- Thinking content display for Claude messages
- Project viewer for Claude projects
- Share functionality (copy chat links)
- Responsive design for mobile/desktop