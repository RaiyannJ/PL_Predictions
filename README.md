# PL_Predictions

Hello! This project combines my passion for Premier League Football and Machine Learning to create a model that predicts the outcomes of Premier League games. Using data from the 2023 and first half of 2024, the model was trained to predict the outcomes of the games during the second half of the 2024 season.

The first step was to scrape data from Fbref football statistics website using various html libraries (requests, BeautifulSoup) and data processing libraries (Pandas, StringIO).

Once the data of all the games played over those seasons (1520 games!) and various statistics from the stadium, the day to deep football stats such as progressive passes, shots on target etc, the data was ready to be cleaned and processed for our use.

The model used was a Random Forest Classifier due to the non-linearity of the data, but it was a basic model, with a precision of about 52%. However after applying a rolling averages method and other data processing steps, this model was trained and arrived at a final test precision of 71% (almost a 20% increase!)

Some key takeaways regarding what stats mattered the most from my analysis and tweaking were that the rolling averages from the previous games of possession, progressive passes, touches in the attacking third and defensive errors were crucial to predicting future games. On the other hand, expected goals/goals allowed and touches did not affect the data!

And of course, Go Liverpool!!!

Project inspiration comes from Dataquest!
