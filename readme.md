# Markdown Editor

A sleek and fast Markdown editor for effortless writing and live preview. Write, edit, and convert Markdown with ease—perfect for developers, writers, and note-takers.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Classes](#classes)
- [Contributing](#contributing)
- [License](#license)

## Overview

**Markdown Editor** is a web-based application that provides a modern, retro-inspired interface for editing Markdown with live preview. It supports GitHub Flavored Markdown, custom table styling, LaTeX math rendering, split/single view toggling, and PDF export.

## Features

- Live preview as you type
- Toggle between split and single view
- Print to PDF functionality
- Custom table styling
- LaTeX math support (via KaTeX)
- Responsive design for desktop and mobile

## Installation

No installation required. Simply open the HTML file in your browser.

To run locally:

1. Clone the repository:
    ```bash
    git clone https://github.com/Hell0Beta/markdown.git
    cd markdown
    ```
2. Open `index.html` in your browser.

## Usage

- Type Markdown in the left pane; see the rendered preview on the right.
- Use the **Split View** button to toggle between split and single view.
- Use the **Print to PDF** button to print or save your document as a PDF.
- Use the **LaTeX: ON/OFF** button to enable or disable LaTeX math rendering.

### Example

```markdown
# Hello Markdown!

This editor supports **bold**, _italic_, `inline code`, and:

- Live preview
- Table rendering
- LaTeX: $E = mc^2$

| Feature      | Description                        |
|--------------|------------------------------------|
| Live Preview | See your markdown rendered live    |
| LaTeX        | Render math equations with KaTeX   |
```

## Classes

### `MarkdownEditor`

Handles the main editor logic, including input, preview, and event management.

- `init()`: Initializes the editor.
- `attachEventListeners()`: Sets up event listeners.
- `updatePreview()`: Renders Markdown to HTML.

### `MarkdownRenderer`

Converts Markdown to HTML and applies custom table styling.

- `renderMarkdown(markdownText)`: Converts Markdown to HTML.
- `applyTableStyling(previewElement)`: Adds styling to tables.

### `ViewManager`

Manages split/single view toggling.

- `toggleView()`: Switches between split and single view.

### `PdfPrinter`

Handles printing the preview as a PDF.

- `printPreviewAsPdf()`: Opens a print dialog for the preview.

### `LaTeXRenderer`

Handles LaTeX math rendering using KaTeX.

- `renderLaTeX(element)`: Renders LaTeX expressions in the preview.

### `EnhancedMarkdownEditor`

Extends `MarkdownEditor` to add LaTeX toggle functionality.

- `toggleLaTeX()`: Enables/disables LaTeX rendering.

## Contributing

Contributions are welcome! Please open issues or submit pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
