# PL_Predictions

Hello! This project combines my passion for Premier League Football and Machine Learning to create a model that predicts the outcomes of Premier League games. Using data from the 2023 and first half of 2024, the model was trained to predict the outcomes of the games during the second half of the 2024 season.

First step was to web scrape data from Fbref football statistics website using various html libraries (requests, BeautifulSoup) and data processing libraries (Pandas, StringIO).

Once the data of all the games played over those seasons (1520 games!) and various different statistics from stadium, day all the way to deep football stats such ass progressive passes, shots on target etc, the data was ready to be cleaned and processed for our use.

The model used was a Random Forest Classifier due to the non-linearity of the data, but was a basic model, with precision of about 52%. But after applying a rolling averages method and other data processing steps, this model was trained and arrived at a final test precision of 71% (almost a 20% increase!)

Some key takeaways regarding what stats mattered the most from my analysis and tweaking was that the rolling averages from the previous games of possession, progressive passes, touches in attacking third and defensive errors were crucial to predict future games. On the otherhand, expected goals/goals allowed and touches did not really affect the data!

Project inspiration comes from Dataquest!