# -Customer-Experience-Analytics
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

