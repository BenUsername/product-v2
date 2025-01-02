# AI Marketing Analytics Dashboard

A modern web dashboard that helps businesses optimize their product visibility in AI-driven search results. The dashboard provides insights into how AI models like ChatGPT perceive and recommend products, along with detailed analytics about user interactions and search patterns.

## Features

1. Interactive Data Display
   - Main table with product information
   - Clickable cells with category-specific details
   - Product column: Shows search keywords when clicked
   - Persona column: Shows detailed persona information when clicked
   - Relevant Searches column: Shows actual GPT conversations when clicked

2. Product Information
   - Product images linked to website
   - Persona summaries
   - Search volume ranges
   - Competitor websites as clickable links
   - Click metrics and conversion rates

3. Visual Design
   - Clean, modern interface with Tailwind CSS
   - Responsive table layout
   - Expandable rows for detailed information
   - Professional typography and spacing

4. Data Structure
   - CSV-based data management
   - Real-time data loading
   - Auto-refresh every 5 minutes
   - Support for multiple data sources

5. Interactive Features
   - Clickable product images linking to product pages
   - Competitor website links in impressions column
   - Expandable details sections
   - Only one details section open at a time
   - Category-specific content display based on clicked column

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/BenUsername/product-v2.git
   cd product-v2
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Build the CSS:
   ```bash
   npm run build
   ```

4. Start the development server:
   ```bash
   npm run serve
   ```

5. Visit `http://localhost:8000` in your browser

## Development

- Run the Tailwind CSS watcher:
  ```bash
  npm run watch
  ```

## Project Structure

```
product-v2/
├── src/
│   ├── index.html      # Main dashboard HTML
│   ├── input.css       # Tailwind CSS input file
│   └── img/            # Image assets
├── data/
│   ├── data.csv        # Main product data
│   ├── brand_sources.csv # Brand source links
│   └── extract_*.csv   # GPT conversation data
├── dist/
│   └── output.css      # Generated CSS
├── package.json
├── tailwind.config.js
└── README.md
```

## Data Files

- `data.csv`: Contains main product information including metrics
- `brand_sources.csv`: Maps brand URLs to their source articles
- `extract_*.csv`: Contains GPT conversations for each product

## Technologies Used

- HTML5
- Tailwind CSS
- JavaScript (Vanilla)
- Papa Parse for CSV handling
- Python's HTTP server for development

## License

ISC 