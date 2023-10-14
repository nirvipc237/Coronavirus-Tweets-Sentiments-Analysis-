# Coronavirus-Tweets-Sentiments-Analysis-
Project Summary - The CoVid-19 pandemic has had a profound impact on society, disrupting lives and livelihoods worldwide. Lockdown measures forced people to stay indoors, leading to significant changes in daily routines and interactions. During these challenging times, Twitter emerged as a prominent platform for people to express their thoughts and emotions, making it an essential source for understanding public sentiments.

Our analysis focused on gauging the sentiments of individuals by analyzing their tweets on Twitter. We aimed to comprehend the prevailing emotions and opinions of people during the pandemic through text data.

Overall, our analysis aimed to understand the sentiments expressed by people on Twitter during the pandemic and explore which machine learning algorithms and vectorization techniques perform best in sentiment classification. By leveraging Twitter data, we gained valuable insights into the prevailing sentiments and emotions of individuals during these unprecedented times.

Problem Statement

In this challenge, we are tasked with building a classification model to predict the sentiment of COVID-19 related tweets. The dataset consists of tweets collected from Twitter, and manual tagging has been performed to label each tweet with its corresponding sentiment.

The information provided in the dataset includes:

-Location: The geographical location associated with the tweet, indicating where it was posted from.

-TweetAt:The timestamp or date when the tweet was posted.

-Original Tweet: The actual text content of the tweet.

-Sentiment: The sentiment label assigned to each tweet, indicating whether it is positive, negative, or neutral in tone.

-User Name: A code or identifier for the Twitter user who posted the tweet, used to maintain privacy and anonymity.

-Screen Name: Another code or identifier for the Twitter screen name of the user who posted the tweet, also used for privacy reasons.

With this dataset, our objective is to develop a machine learning classification model that can analyze the tweet's content and accurately predict its sentiment as either positive, negative, or neutral. By leveraging the provided features, such as the tweet's text content, location, and timestamp, we aim to gain valuable insights into the overall sentiments expressed by Twitter users regarding COVID-19. This model could be valuable for understanding public sentiments during the pandemic and monitoring the emotional response to various events and situations related to COVID-19 on social media.

Variables Description:-

The dataset under consideration contains information about tweets related to the Coronavirus pandemic. It includes valuable attributes extracted from the tweets, which can aid in understanding public sentiments, opinions, and geographical distribution during the pandemic. The dataset consists of several columns, each holding specific information about the tweets and the users who posted them. The columns include UserName, ScreenName, Location, TweetAt, OriginalTweet, and Sentiment. Let's explore each of these columns to gain insights into the data and better comprehend the characteristics of the tweets in this dataset:

UserName: This column contains the username of the person who authored the tweet on Twitter.

ScreenName: This column contains the screen name or handle of the Twitter user who posted the tweet.

Location: This column represents the location information provided by the Twitter user in their profile. It may include details about their city, state, country, or any other geographic location they have specified.

TweetAt: This column stores the date and time when the tweet was posted on Twitter.

OriginalTweet: This column contains the actual content of the tweet that was posted by the user.

Sentiment: This column contains the sentiment label assigned to the tweet based on the results of a sentiment analysis algorithm. The sentiment label can indicate whether the tweet's content is positive, negative, extremely positive, extremely negative, or neutral, depending on the sentiment analysis results.

The dataset's attributes offer a comprehensive view of the tweets, allowing us to explore public sentiments, identify tweet patterns, and potentially build a classification model to categorize tweets based on their sentiment.

Data Wrangling Code

As we are focusing on classifying tweets based on the text in the 'OriginalTweet' column, we do not need to remove null values from the 'Location' column. Retaining the null values in the 'Location' column ensures that we don't lose any potentially valuable information that could be useful for our classification model. Removing null values from 'Location' might lead to a loss of geographic information and could potentially impact the effectiveness of our model in understanding the relationship between tweet content and geographical location. Therefore, we choose to retain the null values in the 'Location' column to preserve all available data for our classification task.

What all manipulations have you done and insights you found?

Understanding the dataset's structure and contents is crucial for conducting a thorough analysis. To achieve this, several data preparation steps are taken, including:

Identifying Column Names: The first step involves identifying the names of each column present in the dataset.

Describing Columns: Each column is then described with pertinent details such as data type, possible value ranges, and other relevant information.

Defining Variables: In this stage, the variables in the dataset are characterized, including their types (numerical, categorical, etc.) and their respective roles or functions.

Verifying Unique Values: The dataset is checked for unique values within each column to identify any potential duplicates.

Managing Null Values: It is noted that there is no need to remove or delete the empty values (null values), as they are retained in the analysis.

By conducting these data preparation processes, we gain a comprehensive understanding of the dataset's attributes, enabling us to proceed with the analysis and build effective models for classification or any other desired tasks.

Conclusion

We have evaluated and compared eight different models for sentiment analysis, including Logistic Regression with Grid Search CV, Decision Tree Classifier, Stochastic Gradient Descent, KNN, SVM, Multinomial Navies Bayes, and Bernoulli Navies Bayes classifiers. We applied these models with both Count Vectorization and TF-IDF Vectorization techniques to transform the text data into numerical representations.

After analyzing the results, we have determined that the Stochastic Gradient Descent model with Count Vectorization achieved the highest accuracy of 80.43%. It outperformed all other models in accurately classifying sentiments across different categories (negative, neutral, positive). The second-best performer was the Logistic Regression with Grid Search CV model using TF-IDF Vectorization, which achieved an accuracy of 78.86%.

The results demonstrate that the Stochastic Gradient Descent model with Count Vectorization is the most suitable choice for sentiment analysis in this specific dataset. Its high accuracy level indicates its capability to make reliable predictions, making it a valuable tool for understanding public sentiment, customer feedback, and opinion analysis across various domains.

We can confidently deploy the selected Stochastic Gradient Descent model with Count Vectorization for sentiment analysis tasks in real-world applications. Its accuracy and overall performance make it a robust and dependable solution for understanding sentiments expressed in textual data.

It is crucial to monitor and reevaluate the model's performance over time to ensure its continued effectiveness. In the future, we can repeat the sentiment analysis and compare it with the present analysis to gauge the impact of any changes or initiatives on sentiments expressed by the target audience.

By regularly updating and retraining the model with new data, we can maintain its relevance and adaptability to evolving sentiment patterns in the dataset.

Additionally, we can explore other advanced natural language processing techniques and deep learning models to further improve sentiment analysis accuracy and gain deeper insights into text data.

Careful consideration of feature selection and engineering can play a crucial role in enhancing the model's performance. Analyzing feature importance using techniques like Permutation Importance can help identify critical words or phrases that drive sentiment predictions.

Conducting a thorough error analysis can provide valuable feedback on the model's weaknesses and areas for improvement. This can guide the refinement of the model and lead to more accurate predictions in future iterations.

The choice of evaluation metrics should align with the specific objectives and requirements of the sentiment analysis task. For example, if identifying negative sentiments is more critical in a particular application, then prioritizing recall for the negative class might be more appropriate.

Regular monitoring of the model's performance against new data and comparing it with the initial results can help detect potential biases or changes in sentiment distribution over time.

Deploying sentiment analysis models in real-world applications should consider ethical implications and potential bias in the training data. Ensuring fairness and avoiding unintended consequences are essential aspects of responsible AI deployment.

Collaboration with domain experts, stakeholders, and end-users can provide valuable feedback and domain-specific insights to enhance the model's accuracy and relevance.

Continuously staying updated with advancements in natural language processing and machine learning can open up new opportunities for refining sentiment analysis models and staying at the forefront of research and technology.

The chosen model's performance and insights obtained from sentiment analysis can drive actionable decisions and inform strategies across various industries, including market research, customer service, social media analytics, and brand reputation management.
