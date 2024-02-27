# sentiment-analysis
Using Machine Learning
Sentiment analysis is a powerful machine learning tool that enables the automated identification of attitudes, opinions, and emotions expressed in text. 
In this study, we explore the application of sentiment analysis to evaluate the learning experiences. 
Specifically, we investigate whether sentiment analysis algorithms can effectively replace multiple human raters in research.

Our dataset comprises evaluations from 421 feedback of people opinion on their experiences. 
The sentiments expressed in these evaluations were categorized as positive, negative, or neutral,which is further classified from humour to hate in this project.

Machine Learning Models: Various algorithms can be employed for sentiment analysis:
Here we use Naive Bayes: A probabilistic classifier often used for text classification.

Our findings reveal the following:
Naive Bayes achieved an impressive 98% accuracy when excluding neutral sentiments.

Function called categorize_sentiment that categorizes sentiment scores based on predefined thresholds. 
The function takes a compound score as input, which represents the overall sentiment polarity of a text (e.g., a review, tweet, or comment).

Function Description
The categorize_sentiment function operates as follows:

Input: The function receives a single argument, compound, which is a floating-point value ranging from -1.0 (most negative sentiment) to 1.0 (most positive sentiment).

Thresholds: We define several sentiment categories and associated thresholds:

Humor: Compound score ≥ 0.8
Praise: Compound score ≥ 0.6
Gratitude: Compound score ≥ 0.4
Excitement: Compound score ≥ 0.2
Fair: Compound score < 0.2 (but not negative)
Sad: Compound score < -0.2 (negative sentiment)
Jealous: Compound score < -0.6
Hate: Compound score < -0.8

Categorization: The function iterates through the thresholds and assigns the appropriate sentiment label based on the compound value. If no threshold is met, the default label is “anger.”

Output: The function returns the determined sentiment category.

Conclusion
The categorize_sentiment function provides a simple yet effective way to classify sentiment scores, making it useful for various natural language processing tasks.

Applications of Sentiment Analysis:
Social Media Monitoring: Brands analyze social media posts to gauge public sentiment about their products or services.
Customer Reviews: E-commerce platforms use sentiment analysis to understand customer feedback.
Financial Markets: Sentiment analysis helps predict stock market trends based on news sentiment.
Political Analysis: Analyzing political speeches, tweets, and news articles to assess public opinion.
Healthcare: Identifying patient sentiments from medical records or online health forums.

In summary, sentiment analysis is a powerful tool that enables us to extract valuable insights from textual data.
Whether it’s improving customer experiences, tracking brand reputation, or understanding public sentiment, sentiment analysis plays a crucial role in today’s data-driven world.
