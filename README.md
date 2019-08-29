# Improve Natgeo Instagram Engagement

Acadamic project from class User Generated Content Analytics.

Is a Picture Worth a Thousand Words?

Goal:

On Instagram, choose the National Geographic (natgeo) page (do not use hashtags). Write a scraper or use the Web Scraper to extract (i) image URLs (no video URLs), (ii) post caption (the text description of a post), (iii) # likes and (iv) # comments. Scrape 250-500 image posts. 

Based on the mesagges scraped from Instagram, find insights on improving user engagement.


## Data

json file:
- posts.json: text description of a post


## Tasks Completed:

1. Create a metric for engagement by using a weighted sum of # likes and # comments. First, normalize # likes and # comments such that they both have values between 0 and 1. (scale the # likes by dividing by the maximum # likes (for a post) as well as for # comments.) Then create an engagement score = .4*# likes (normalized) + .6*# comments (normalized). Define High (1) and Low (0) engagement based on whether the engagement score is above or below the median value.  

2. Run a logistic regression with Engagement (binary) as the dependent variable, and the image labels as independent variables. Find the accuracy and show the confusion matrix.

3. Perform topic modeling (LDA) on the image labels. LDA produces two outputs: (i) A file showing which words load on which topics, and (ii) a file showing topic weights for each image. 
Take the quartiles with highest and lowest engagement scores, find the differences in the average topic weights of pictures across the two quartiles (e.g., greater proportion of some topics in highest engagement quartile).

4. Provide advice for National Geographic to increase engagement on its Instagram page.

