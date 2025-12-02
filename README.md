# -Customer-Experience-Analytics

Insights, Visualizations & Recommendations
Objective

Analyze sentiment, identify themes, and visualize customer experience insights using Python.

Steps Performed
1. Insights Extraction

Extracted sentiment per bank

Identified keyword-based themes (speed, crashes, usability, login issues)

Found:

Drivers (e.g., fast service, easy navigation)

Pain Points (e.g., crashes, login failures)

2. Visualizations Created

Rating distribution per bank

Sentiment distribution per bank

Word cloud (positive reviews)

Word cloud (negative reviews)

3. Recommendations

Per bank, we propose improvements such as:

Speed optimization

Crash reduction

Better login workflow

Enhanced app usability

Ethical Considerations

Google Play reviews are biased toward dissatisfied users.

Not all reviews represent typical users; some may be spam or duplicates.

Sentiment models are not perfect and may misclassify sarcasm or mixed feedback.
Database: bank_reviews

Table: banks
- bank_id (SERIAL PRIMARY KEY)
- bank_name (VARCHAR UNIQUE)
- app_name (VARCHAR)

Table: reviews
- review_id (SERIAL PRIMARY KEY)
- bank_id (INT, FOREIGN KEY -> banks.bank_id)
- review_text (TEXT)
- rating (INT)
- review_date (DATE)
- sentiment_label (VARCHAR)
- sentiment_score (FLOAT)
- source (VARCHAR)

# Customer Experience Analytics

This project collects, preprocesses, and analyzes customer reviews from the Google Play Store for Ethiopian banks. The goal is to clean the data and prepare it for further analysis and modeling.

## Project Structure

