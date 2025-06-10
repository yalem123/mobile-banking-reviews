# Task 1: Data Collection and Preprocessing

## Objective

Scrape reviews from the Google Play Store, preprocess them for analysis, and prepare the dataset for further tasks.

## Banks

- Commercial Bank of Ethiopia (CBE)
- Bank of Abyssinia (BOA)
- Dashen Bank

## Process

### Web Scraping

- Used `google-play-scraper` library to collect reviews.
- Collected the following fields:
  - Review Text
  - Rating (1-5)
  - Date (normalized to YYYY-MM-DD)
  - Bank/App Name
  - Source = "Google Play"

### Preprocessing

- Removed duplicate reviews.
- Handled missing data (<5% missing data after cleaning).
- Normalized dates to `YYYY-MM-DD` format.
- Final dataset saved as CSV with columns:
  - `review`
  - `rating`
  - `date`
  - `bank`
  - `source`

### Output

- ✅ Scraped 400+ reviews per bank (over 1200 reviews in total).
- ✅ Saved clean dataset: `clean_reviews.csv`

## Git Process

- Branch: `task-1`
- Frequent commits after each major step:
  - Initial scraper setup
  - First review batch scraped
  - Preprocessing script
  - Clean CSV saved
  - README updated

## Notes

- Limitations of scraping:
  - Some reviews may have limited content.
  - Occasional scraping errors handled with retries.

## Next Steps

Proceed to Task 2: Sentiment and Thematic Analysis.

