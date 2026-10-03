# E-commerce Price Intelligence

E-commerce price tracking and analytics project built to collect, store, and analyze product pricing and availability data from Amazon and Flipkart.

The project tracks historical product data and provides analysis for price changes, competitive pricing, stock availability, and marketplace/category trends.

## Project Overview

The project uses automated web scraping to collect product information from Amazon and Flipkart. The collected data is stored in MySQL and processed using Python and SQL.

The analyzed data is then presented through Excel and Streamlit dashboards for product-level and category-level analysis.

## What the Project Covers

* Product price tracking
* Historical price analysis
* Price change analysis
* Amazon vs. Flipkart price comparison
* Stock availability tracking
* Product-level analysis
* Category-level analysis
* Marketplace dominance analysis
* Interactive dashboards

## Analytical Modules

### Price Change Analysis

Tracks how product prices change over time and includes:

* Initial price
* Current price
* Highest price
* Lowest price
* Price change
* Price change percentage
* Historical price trends

### Competitive Pricing

Compares product prices between Amazon and Flipkart to identify:

* Price differences
* Competitive pricing gaps
* Marketplace-specific pricing
* Product-level comparisons

### Category & Marketplace Analysis

Analyzes products across categories to understand:

* Marketplace presence
* Product availability
* Category distribution
* Platform dominance
* Category-level pricing trends

## Technology Used

| Technology    | Usage                          |
| ------------- | ------------------------------ |
| Python        | Data collection and processing |
| Selenium      | Web scraping                   |
| MySQL         | Data storage                   |
| SQL           | Data analysis                  |
| Pandas        | Data processing                |
| Streamlit     | Dashboard                      |
| Plotly        | Visualizations                 |
| Excel         | Analysis and dashboards        |
| Google Sheets | Product input and management   |

## Data Flow

```text
Google Sheets
     ↓
Amazon / Flipkart
     ↓
Selenium Scraping
     ↓
MySQL
     ↓
Python + Pandas
     ↓
SQL Analysis
     ↓
Excel / Streamlit
     ↓
Insights
```

## Dashboards

The project includes dashboards for:

**Product Intelligence**

* Product KPIs
* Historical prices
* Price changes
* Marketplace comparison
* Product-level analysis

**Category Intelligence**

* Category KPIs
* Marketplace comparison
* Product availability
* Category trends
* Marketplace dominance

## Project Structure

```text
ecommerce-price-intelligence/
│
├── scraper/
│   ├── amazon_scraper.py
│   ├── flipkart_scraper.py
│   ├── final_pipeline.py
│   ├── parallel_pipeline_experimental.py
│   ├── website_home.py
│   ├── website_databases.py
│   ├── website_product_dashboard.py
│   ├── website_product_intelligence_route.py
│   ├── website_full_category_intelligence_dashboard.py
│   ├── website_insights_product_intelligence_dashboard.py
│   └── website_insights_category_intelligence_dashboard.py
│
├── screenshots/
│
├── requirements.txt
└── README.md
```

## Running the Project

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/ecommerce-price-intelligence.git
cd ecommerce-price-intelligence
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Configure the MySQL database connection and required product inputs.

Run the scraping pipeline:

```bash
python scraper/final_pipeline.py
```

Run the Streamlit dashboard:

```bash
streamlit run scraper/website_home.py
```

## Project Objective

The main objective of the project is to turn marketplace data into useful pricing and competitive insights by combining web scraping, database management, SQL analysis, and visualization.



