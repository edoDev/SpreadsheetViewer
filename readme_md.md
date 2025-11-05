# 📊 Spreadsheet Viewer

A lightweight, browser-based spreadsheet viewer with sorting, deduplication, and theme support. No installation required - just open and use!

![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)

## ✨ Features

- 📁 **Multiple File Format Support**
  - CSV (Comma-Separated Values)
  - TSV (Tab-Separated Values)
  - XLSX (Excel 2007+)
  - XLS (Excel 97-2003)
  - ODS (OpenDocument Spreadsheet)

- ⬆️⬇️ **Sortable Columns**
  - Click any column header to sort
  - Toggle between ascending and descending order
  - Smart sorting (detects numbers vs text)

- 🔄 **Column Deduplication**
  - Remove duplicate values from individual columns
  - Click "✓ Dedupe" on any column header
  - Keeps first occurrence, removes subsequent duplicates
  - Reset data to original state anytime

- 🌓 **Theme Support**
  - Dark mode (default)
  - Light mode
  - Smooth transitions between themes
  - Persistent preference

- 🎨 **Modern UI**
  - Clean, responsive design
  - Smooth animations
  - Mobile-friendly
  - No dependencies beyond included libraries

## 🚀 Getting Started

### Quick Start

1. Download the `spreadsheet-viewer.html` file
2. Open it in any modern web browser
3. Click "Choose File" and select your spreadsheet
4. Start exploring your data!

### Usage

```bash
# Option 1: Open directly
Double-click the HTML file

# Option 2: Serve locally
python -m http.server 8000
# Then open http://localhost:8000/spreadsheet-viewer.html

# Option 3: Use with any web server
```

## 📖 How to Use

### Loading Files
1. Click the **"📁 Choose File"** button
2. Select a CSV, TSV, XLSX, XLS, or ODS file
3. Your data will appear in the table

### Sorting Data
- Click any column header to sort by that column
- Click again to reverse the sort order
- The arrow indicator shows current sort direction (↑ or ↓)

### Removing Duplicates
1. Click the **"✓ Dedupe"** button in any column header
2. Rows with duplicate values in that column will be removed
3. The first occurrence of each value is kept
4. A notification shows how many rows were removed

### Resetting Data
- Click **"↺ Reset Data"** to restore the original dataset
- This undoes all deduplication operations

### Changing Theme
- Toggle the switch in the top right (☀️/🌙)
- Switch between light and dark modes

## 🛠️ Technical Details

### Built With
- **PapaParse** (5.3.2) - CSV/TSV parsing
- **SheetJS** (0.18.5) - Excel file handling
- Vanilla JavaScript (no frameworks)
- Modern CSS with smooth transitions

### Browser Compatibility
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Any modern browser with ES6 support

### File Size Limits
- Handles files up to several MB comfortably
- Performance depends on browser and system memory
- Large files (10,000+ rows) may take a moment to process

## 🔒 Privacy

- **100% client-side processing** - all data stays in your browser
- No data is uploaded to any server
- No tracking or analytics
- No internet connection required after initial load

## 📝 Examples

### Deduplicating Customer Data
1. Load your customer list CSV
2. Click "✓ Dedupe" on the "Email" column to remove duplicate customers
3. Sort by "Name" to organize alphabetically

### Analyzing Survey Results
1. Import your survey XLSX file
2. Sort by "Response Date" to see chronological order
3. Dedupe by "User ID" to get unique respondents

### Cleaning Product Lists
1. Load your inventory spreadsheet
2. Dedupe by "SKU" to remove duplicate products
3. Sort by "Price" to analyze pricing

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Ideas for Contributions
- Export functionality (download cleaned data)
- Column filtering
- Search functionality
- Column width adjustment
- Multi-column sorting
- Regular expression filtering
- Statistics/summary view
- Custom theme colors

## 📋 Roadmap

- [ ] Export cleaned data to CSV/XLSX
- [ ] Column filtering capabilities
- [ ] Search across all columns
- [ ] Keyboard shortcuts
- [ ] Column reordering
- [ ] Cell editing
- [ ] Formula support
- [ ] Chart visualization

## 🐛 Known Issues

- Very large files (100,000+ rows) may cause browser slowdown
- Sheet selection not available for multi-sheet Excel files (uses first sheet only)
- Mobile support is functional but not optimized

## 📄 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [PapaParse](https://www.papaparse.com/) - Fast CSV parser
- [SheetJS](https://sheetjs.com/) - Excel file processing
- Inspired by the need for simple, privacy-focused data tools

## 📧 Contact

If you have questions or suggestions, please open an issue on GitHub.

---

**Made with ❤️ for data enthusiasts who value simplicity and privacy**