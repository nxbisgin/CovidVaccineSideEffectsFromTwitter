https://medium.com/@neslihanbisgin/mining-twitter-to-explore-the-odds-of-having-side-effects-after-covid-vaccine-4c3f0f35392c

Mining Twitter to explore the odds of having side effects after COVID vaccine

According to CDC, you may have some side effects after getting a COVID-19 vaccination such as pain, redness, swelling on the arm and tiredness, headache, muscle pain, chills, fever and nausea throughout the rest of your body. Before taking the COVID shot, I was wondering how likely am I to experience these side effects, or which ones I will have. On the other hand, some people have no side effects. How likely am I to be one of those lucky people? I asked my friends who took the shot before me but I realized I needed more data, so I turned to Twitter.

Possible side effects after COVID vaccine.
Social media data can produce rich and useful insights in both scale and extent. With people sharing their vaccine experience in real time, Twitter was the perfect source of data for me.
Sample of tweets that were collected.
With a quick search, I found a dataset already available on Kaggle related to vaccine tweets so I decided to use it to answer my questions. The data was collected using Tweepy Python package to access Twitter API and most frequently used terms to refer to the vaccines were used for collection. The tweets date back to 12/31/2020 and it is frequently updated to add more recent tweets. For more details about the dataset, you can visit the link here.
Here is a quick summary of my research questions:
1. What is the possibility that your shot is largely uneventful?
2. Which side effects are more rare/common?
3. Can social media aid as a way to track rare/unknown side effects?
I started by downloading the data and cleaning the tweets. There were 168,224 tweets in the dataset (limited number available due to Twitter API). As a preprocessing step, I removed urls, emojis, numbers, punctuation marks and any word that is less than 3 character long, then converted all text to lowercase. Below is a word cloud for the cleaned tweets to give an idea about the conversation.

Word Cloud for All Tweets
Since, I was interested on the number of mentions for each side effect, I needed to further process the data and get the word counts. I started by tokenizing the cleaned tweets and then created a word counter in clean tweets. If the word is one of the side effect related terms and if the word count is greater than 50, it is shown in the bar plot below.

According to the results, people mentioned the word “sore” in 16% of the side effect related tweets and the word “soreness” in 3%, which is possibly referring to the “sore arm” or “soreness in the arm”. If the words “swollen”, “swelling” and “tender” are also included in this category (with the assumption that they are used to describe the pain in the arm), swollen or sore arm makes 22% of all the reported side effects.
Fever was reported in 8% of the side effect related tweets and chills was reported in 4% of them. Headache was reported 7% of the time (combination of words “headache” and “headaches”). Fatigue was another common side effect making 8% of all reported side effects (combination of words “tired”, “fatigue” and “fatigued”). Also, blood clots were mentioned in 8% of them (combination of words “bloodclot”, “clots”, “clot” and “clotting”). Heart was mentioned in 5% of the tweets and vision was mentioned in 4%, which may indicate a problems related to heart and vision. Other side effects mentioned are: inflammation (3%), myocarditis (1%), some problem about periods (1%) and nausea (1%). These are some of the rare side effects and Twitter data may aid in tracking these side effects. On the other hand, 1% of the related tweets used the word “painless”, so we understand that there were some lucky people who reported a pain free experience.
In case you are wondering, I was not one of those few luckiest people with no side effect. I had a terrible headache, fever, chills and fatigue and of course a swollen arm. All in all, I still feel lucky to have a chance to have the vaccine. Another question in my mind is about the severity of women’s side effects compared to men’s (for more detailed information follow this link). One can compare women’s side effects to men’s using Twitter, but that will be a project for later.







