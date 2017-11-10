---
layout: post
title: Find Your Dream Job in Data Science
---
## Why this topic?

Hard to believe that 2/3 of the bootcamp has already past. As the graduation day coming closer, I start to think about job searching. 

It's not an easy process, by doing this project, I hope I could have more insights on:
1. Which are industries that have data science related posting?
2. Who are the top employers?
3. What the key skill sets that they are looking for?
4. How to efficiently find the job that fits me the best?


## Data Source and size

I scraped my data around 900 active job postings from glassdoor.com using the key word "Data Scientist" in Seattle area. For each posting, I obtained the job description, glassdoor estimate salary and several information about the employers include rating, size & revenue. 
   
* Cleaned Data Size:

1. Remove 
  

## Modeling Results

After trying different classification models include KNN, Random Forest, Logistic Regression, Naive Bayes, SVM, Gradient Boosting and Ada Boosting, I found Ada Boosting gave me the best & most consistent results. Below shows the ROC of the test set (0.3 train/test split).
![](/images/Modeling_Result.png?raw=true)
As you can see the AUC is 0.824. Since my data is so biased(only 0.1% of data point is True), The orginal prediction model output from scikit learn pretty much is guessing every city as not having a mass shooting event. :(
That's not gonna help me find the high risk cities.
So along the ROC curve, I picked a cut point that provides a reasonable balance between the false positive rate and the true positive rate. This way, I will be able to identify 75% of the cities that actually had a mass shooting occurred. 

## Findings

https://public.tableau.com/views/Metis-Project4/FindYourDreamJobinDataScience?:embed=y&:display_count=yes&publish=yes



## Future Works 
. 



