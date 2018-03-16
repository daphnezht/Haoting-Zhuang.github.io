---
layout: post
title: NLP Project - Find Your Dream Job in Data Science
---
Hard to believe that 2/3 of the bootcamp has already past. As the graduation day coming closer, I start to think about job searching. 

It's not an easy process. By doing this NLP project, I hope I could have more insights on:
1. Which are industries that have data science related posting?
2. Who are the top employers?
3. What the key skill sets that they are looking for?
4. How to efficiently find the jobx that fits me the best?


## Data Source and size

I scraped my data around 900 active job postings from glassdoor.com using the key word "Data Scientist" in Seattle area. For each posting, I obtained the job description, glassdoor estimate salary and several information about the employers include rating, size & revenue. 


## Modeling Steps   

* Text Pre-processing:

1. Retrieved all the skill sets related information and counted how frequently each skill appears in the job description(e.g., Python, R).
2. Retrieved sentences which mentioned "year...experience". From there, got the required number of years of experience.
3. Remove all the non-alphabetic characters and stop words. Change the text to lower case. 
3. Remove company names from the job description.
4. Remove common words especially for the ones in section where employers talk about being an equal opportunity employer.
5. Use TF-IDF 2-3 ngrams to tokenized the job description cleaned by the previous two steps.

* Topic Modeling:

1. Initially I was having trouble identifying clear topics. When I used LSA to split the full dataset sets into two topics. I found one is related to medical laboratory research, while the other one is more data science related. Below shows the scatter plot with x & y as the two LSA topic probabilities. Therefore I removed the datapoints related to medical laboratory research (around 100 datapoints). After that, the topic modeling become more clear. 
![](/images/LSA_split_to_2.png?raw=true) 

2. I tried a few techniques include LDA, LSA and NMF. And the one give me the best result is 4-topic-split using NMF. Below I have created a Tableau story book showing the results of exploration data analysis and topic modeling. 
 
Findings

<iframe src="https://public.tableau.com/views/Metis-Project4/FindYourDreamJobinDataScience?:embed=y&:display_count=yes&publish=yes"
 width="700" height="1200"></iframe>

[Here is also the link to my Tableau storybook if you have trouble viewing](https://public.tableau.com/views/Metis-Project4/FindYourDreamJobinDataScience?:embed=y&:display_count=yes&publish=yes)

* Recommendation System

I read in my resume in plain text format, did the same text processing as the job descriptions, and then I calculated the cosine similarity between my resume and all the job descriptions. Below are the ones with top similarity scores.

![](/images/Recommendation_result.png?raw=true) 

## Future Works 

In the future, I would like to:
1. Do more data exploration analysis
2. Build UI for job recommendation system
3. Refine recommendation system by incorporating user application history



