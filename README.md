# Task 2: Sentiment and Thematic Analysis

## Objective

Quantify review sentiment and identify key themes to uncover satisfaction drivers and pain points for each bank.

## Steps

### Sentiment Analysis

- Used VADER SentimentIntensityAnalyzer for initial sentiment scoring.
- For each review:
  - Computed compound sentiment score.
  - Labeled as:
    - Positive
    - Neutral
    - Negative
- Aggregated sentiment scores by:
  - Bank
  - Rating

### Thematic Analysis

#### Keyword Extraction

- Used TF-IDF vectorizer to extract top keywords per bank.
- Keywords reviewed and grouped manually into themes.

#### Themes Defined

Example themes per bank (actual themes documented in final report):

- Account Access Issues
- Transaction Performance
- User Interface & Experience
- Customer Support
- Feature Requests

#### Theme Mapping

- Applied rule-based mapping to assign themes back to individual reviews.
- Created new column: `identified_theme(s)`.

### Output

- Sentiment aggregation saved: `sentiment_aggregated_by_bank_rating.csv`
- Final reviews with themes saved: `final_reviews_with_themes.csv`

### Git Process

- Branch: `task-2`
- Frequent commits after each major step:
  - Sentiment scoring implemented
  - Aggregation by bank and rating
  - TF-IDF extraction + theme table prepared
  - Theme mapping script implemented
  - Final CSV saved
  - README updated

## Notes

- Some reviews contain mixed topics → simple rule-based mapping used.
- Manual review of themes was performed to ensure relevance.

## Next Steps

Proceed to Task 3: Store Cleaned Data in Database.

