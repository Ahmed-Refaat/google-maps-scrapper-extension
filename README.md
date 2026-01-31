# 🗺️ Google Maps Scraper Extension

A Chrome extension that allows you to easily scrape business information from Google Maps search results and export the data to CSV format.

## 📋 Features

- **Easy Scraping**: One-click scraping of Google Maps search results
- **Comprehensive Data**: Extracts multiple data points from each business listing
- **CSV Export**: Download scraped data as CSV with custom filename
- **User-Friendly Interface**: Clean and intuitive popup interface
- **Real-time Preview**: View scraped data in a table before downloading

## 📊 Data Extracted

The extension scrapes the following information for each business:

- **Title**: Business name
- **Rating**: Star rating (out of 5)
- **Reviews**: Number of reviews
- **Phone**: Contact phone number
- **Industry**: Business category/type
- **Address**: Physical address
- **Website**: Company website URL
- **Google Maps Link**: Direct link to the Google Maps listing

## 🚀 Installation

### From Source

1. Clone this repository:
   ```bash
   git clone https://github.com/Ahmed-Refaat/google-maps-scrapper-extension.git
   ```

2. Open Chrome and navigate to `chrome://extensions/`

3. Enable "Developer mode" (toggle in the top-right corner)

4. Click "Load unpacked"

5. Select the `google-maps-scrapper-extension` folder

6. The extension icon should now appear in your Chrome toolbar

## 📖 How to Use

1. **Navigate to Google Maps**: Go to [Google Maps](https://www.google.com/maps/search/) and perform a search (e.g., "restaurants in New York")

2. **Open the Extension**: Click on the extension icon in your Chrome toolbar

3. **Scrape Data**: Click the "Scrape Google Maps" button to extract data from the current search results

4. **Preview Results**: View the scraped data in the table that appears

5. **Export to CSV**: 
   - Enter a custom filename (optional)
   - Click "Download as CSV" to save the data

## 💡 Tips

- **Multiple Pages**: To scrape more results, scroll down on Google Maps to load more businesses, then click "Scrape Google Maps" again
- **Custom Filenames**: Enter a descriptive filename before downloading (e.g., "nyc_restaurants")
- **Valid Pages Only**: The extension only works on Google Maps search result pages

## 🛠️ Technical Details

- **Manifest Version**: 3
- **Permissions**: 
  - `activeTab`: Access to the current tab
  - `scripting`: Ability to inject scraping script
- **Browser**: Chrome (Manifest V3 compatible)

## 📁 File Structure

```
google-maps-scrapper-extension/
├── manifest.json       # Extension configuration
├── popup.html          # Extension popup interface
├── popup.js            # Main scraping logic and functionality
├── map.png             # Extension icon
└── README.md           # This file
```

## 🔍 How It Works

1. The extension detects when you're on a Google Maps search page
2. When activated, it injects a script that:
   - Queries the DOM for business listing elements
   - Extracts data using CSS selectors and regex patterns
   - Parses ratings, reviews, addresses, and contact information
3. Displays the data in a formatted table
4. Allows export to CSV format with custom naming

## ⚠️ Limitations

- Only works on Google Maps search result pages
- Data quality depends on Google Maps' page structure
- May need updates if Google changes their HTML structure
- Scrapes only visible results (scroll to load more)

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## 📝 License

This project is open source and available for personal and educational use.

## 🙏 Credits

Original concept by Mike Powers. Modified and maintained by Ahmed Refaat.

## 📧 Contact

For questions or support, please open an issue on GitHub.

---

**Note**: This tool is for educational purposes. Please respect Google's Terms of Service and use responsibly.
