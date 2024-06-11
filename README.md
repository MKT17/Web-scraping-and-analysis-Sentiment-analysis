# Web-scraping-and-analysis-Sentiment-analysis

### Data Used

- **Source:** Customer reviews of British Airways from [Airline Quality](https://www.airlinequality.com/airline-reviews/british-airways).
- **Attributes:** The dataset consists of a single column of text data, where each row represents a customer review.

### The Analysis Made

1. **Data Collection:**
   - Scraped 1000 reviews from 10 pages of British Airways reviews on Airline Quality.
   - Stored the reviews in a pandas DataFrame.

2. **Data Cleaning:**
   - Removed leading/trailing whitespace and certain symbols (e.g., "|" and verification tags).
   - Checked for missing values and calculated the length of each review.

3. **Descriptive Statistics:**
   - Counted the total number of reviews.
   - Calculated summary statistics for the review lengths.

4. **Text Processing:**
   - Tokenized the reviews into words.
   - Removed custom-defined stopwords and non-alphabetic tokens.
   - Created a frequency distribution of words.

5. **Sentiment Analysis:**
   - Used TextBlob to calculate sentiment scores (polarity) for each review.
![Capture](https://github.com/MKT17/Web-scraping-and-analysis-Sentiment-analysis/assets/152396111/9f6b041d-0a34-4ca4-b1af-466ac4147483)

   - Identified the most positive and most negative reviews based on polarity scores.

5. **Visualization:**
   - Plotted the distribution of review lengths.
  
![image](https://github.com/MKT17/Web-scraping-and-analysis-Sentiment-analysis/assets/152396111/2a536e99-2c45-40be-8b03-20d1dc8d9ab2)

   - Generated a word cloud to visualize the most common words in the reviews.

![image](https://github.com/MKT17/Web-scraping-and-analysis-Sentiment-analysis/assets/152396111/e6bbc301-f80e-4138-8aaf-04c6601138cc)

### The Findings

1. **Descriptive Statistics:**
   - Total number of reviews: 1000.
   - Average review length: 816 characters.
   - Review length ranged from 132 to 3466 characters.

2. **Frequent Words:**
   - Most common words: "flight", "ba", "service", "london", "seat", "crew", "class", "food", "british", "airways".

3. **Sentiment Analysis:**
   - Average sentiment (polarity) score: 0.067.
   - Most positive review: "Gatwick to St Lucia. Great service on this flight. Thank you very much for the cabin and the great cabin crew. Excellent Service."
   - Most negative review: "Mykonos to London flight delayed and waiting to depart. They are not on time, be prepared to miss your connections, take off 2 hours late,. The staff is some of the worst I have had on airlines. You may be stuck on the runway and they won’t offer you any water. The worst business class experience I have had."

### The Summary

The analysis involved scraping customer reviews of British Airways, cleaning and processing the text data, performing sentiment analysis, and visualizing the results. Most reviews were relatively short, with an average length of 816 characters. The sentiment of the reviews was generally positive, as indicated by the average sentiment score of 0.067. Common themes in the reviews included service quality, seating, crew behavior, and food.

### The Limitations

1. **Data Source:**
   - The data scraping method may miss some reviews or introduce biases based on page structure and content.

2. **Text Processing:**
   - Custom stopwords list may not capture all irrelevant words, potentially affecting word frequency analysis.

3. **Sentiment Analysis:**
   - The analysis did not account for context or sarcasm, which can affect sentiment interpretation.

4. **Generalizability:**
   - Findings are specific to British Airways reviews on Airline Quality and may not generalize to reviews from other airlines or platforms.
   - Further analysis is needed to compare sentiments across different review sources or airlines.
