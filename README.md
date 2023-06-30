# Airbnb_Boston
Analysis of Airbnb Boston dataset

Trying to find what to do and what not to do as someone who wants to gain profit from Airbnb in Boston:

1) What is Airbnb: it is a website that allows any individual to lease a property for a short duration, Airbnb business model is based on charging a commission on the leasers.

2) The data consists of three data sets (The data timeframe is one year): a listings data set which has all the information shown on the website about the property, a reviews data set that contains all the people's reviews regarding the property, and a calendar data set which when the property was available and when it was not

3) Cleaning and wrangling: The data was cleaned and prepared as seen in the Jupyter notebook attached in the respiratory: I have tried to find the positivity of a comment in a very basic way, I have gathered a list of positive and negative adjectives, then found the ratios of positive and negative adjectives to the length of the comment, then the data was aggregated as an average for each specific property, the new reviews dataset is attached in the respiratory

4) Modeling: The data was modeled to find the best predictors for the response obtained from the calendar dataset which is "not_available_rate", it is assumed that if the property is not available on a certain day then it is leased, the higher the value the better, then the reviews data set and relevant columns in the listing dataset were used to predict the response.

5) Results: after multiple iterations the final model explains 21% of the variation in the response variable, there might be more factors that contribute to the "not_available_rate" rather than the website itself.

6) Some suggestions were made at the end of the notebook and in the Medium post found below.

7) Sources and links:

   Positive words list: https://gist.github.com/mkulakowski2/4289437
   
   Negtive words list: https://gist.github.com/mkulakowski2/4289441
   
   P-value calculator: https://www.datacourses.com/find-p-value-significance-in-scikit-learn-3810/
   
   Medium Post: https://medium.com/@faris.majdali/are-you-leasing-in-boston-b1df9c009e87
