## Project Description
Mobile apps are everywhere. They are easy to create and can be lucrative. Because of these two factors, more and more apps are being developed. In this project, I will do a comprehensive analysis of the Android app market by comparing over ten thousand apps in Google Play across different categories. I'll be looking for insights in the data to devise strategies to drive growth and retention. The data for this project was scraped from the Google Play website. While there are many popular datasets for Apple App Store, there aren't many for Google Play apps, which is partially due to the increased difficulty in scraping the latter as compared to the former. The data files are as follows:<br>

* apps.csv: contains all the details of the apps on Google Play. These are the features that describe an app.<br>
* user_reviews.csv: contains 100 reviews for each app. The text in each review has been pre-processed, passed through a sentiment analyzer engine and tagged with its sentiment score.<br><br>
## Analysis conclusion:<br>
1)There are 33 unique app categories present in our dataset. Family and Game apps have the highest market prevalence. Interestingly, Tools, Business and Medical apps are also at the top.<br>
![fig1](https://user-images.githubusercontent.com/60573989/130359877-76e5f762-6973-42af-8092-8951c1e05e92.png)
<br><br>
2)The average volume of ratings across all app categories is 4.17. The histogram plot is skewed to the left indicating that the majority of the apps are highly rated with only a few exceptions in the low-rated apps.<br>
![fig2](https://user-images.githubusercontent.com/60573989/130359899-315dafca-1bc4-4b78-a851-5ab347031b63.png)
<br><br>
3)The majority of top rated apps (rating over 4) range from 2 MB to 20 MB. We also find that the vast majority of apps price themselves under $10.<br>
![App_rating_vs_App_size(fig3)](https://user-images.githubusercontent.com/60573989/130359942-d4c13e58-0f7f-43b7-b8d7-5d2b02dbd26b.png)
<br>![App_rating_vs_App_Price(fig4)](https://user-images.githubusercontent.com/60573989/130359945-b5b0cb96-3842-4a39-84f0-b037a3388bd7.png)
<br><br>
4)Medical and Family apps are the most expensive. Some medical apps extend even up to $80! All game apps are reasonably priced below $20.<br>
![fig5](https://user-images.githubusercontent.com/60573989/130359995-e64f1750-4514-4326-b4a2-61bc949812db.png)
<br><br>
5)With some more filtering to eliminate "junk" apps, apps of type "Family" seem to be the ones that are mostly paid for prices under 100$.<br>
![fig6](https://user-images.githubusercontent.com/60573989/130360074-243e8bc2-3a61-4e2b-8e24-bd2490efb354.png)
<br><br>
6) paid apps have a relatively lower number of installs than free apps, though the difference is not as stark as I would have expected!<br>
 ![fig7](https://user-images.githubusercontent.com/60573989/130360114-b8302c54-7d4d-4a1b-baa5-157a84172bc6.png)<br><br>
7) Mining user review data to determine how people feel about your product, brand, or service can be done using a technique called sentiment analysis. User reviews for apps can be analyzed to identify if the mood is positive, negative or neutral about that app. For example, positive words in an app review might include words such as 'amazing', 'friendly', 'good', 'great', and 'love'. Negative words might be words like 'malware', 'hate', 'problem', 'refund', and 'incompetent'.<br>

By plotting sentiment polarity scores of user reviews for paid and free apps, I observe that free apps receive a lot of harsh comments, as indicated by the outliers on the negative y-axis. Reviews for paid apps appear never to be extremely negative. This may indicate something about app quality, i.e., paid apps being of higher quality than free apps on average. The median polarity score for paid apps is a little higher than free apps, thereby syncing with our previous observation.<br>![fig8](https://user-images.githubusercontent.com/60573989/130360215-00ba2d6f-384a-431a-a558-58fbe7bfd797.png)

