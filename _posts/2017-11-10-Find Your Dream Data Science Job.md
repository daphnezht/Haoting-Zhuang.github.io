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
2. Remove company names from the job description 
3. Remove common words especially for the ones in section where employers talk about being an equal opportunity employer.

* Topic Modeling:

1. Initially 




* Findings

<iframe src="https://public.tableau.com/views/Metis-Project4/FindYourDreamJobinDataScience?:embed=y&:display_count=yes&publish=yes"
 width="700" height="1200"></iframe>

[Here is also the link to my Tableau storybook if you have trouble viewing](https://public.tableau.com/views/Metis-Project4/FindYourDreamJobinDataScience?:embed=y&:display_count=yes&publish=yes)

* Recommendation System


| Cosine Similarity| Job Title     | Company  | Industry  | Job Highlight  |
|                  |               |          |           |                |
| ---------------- |:------------- | :--------|:----------|:---------------|
|  Human Computer Interaction and Visualization Scientist
                |               |          |           |                |
|                  |               |          |           |                |
|                  |               |          |           |                |
|                  |               |          |           |                |
|                  |               |          |           |                |

## Future Works 




