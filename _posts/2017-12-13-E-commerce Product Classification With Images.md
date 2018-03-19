---
layout: post
title: E-commerce Product Classification With Images
---
## Background
Retail e-commerce share has been growing with a incredible fast pace. For US, in 2016, online sales of physical goods
amounted to 360.3 billion US dollars and are projected to surpass 603.4 billion
US dollars in 2021. The United States rank behind several countries in terms of e-commerce sales as
percentage of total retail sales - in 2016, almost a fifth of China's retail
sales occurred via the internet, compared to only 8.1 percent in the United
States. The UK, South Korea, and Denmark are also ahead of the U.S. in terms of
retail e-commerce share.

## Data Source and size

The image dataset is from a Kaggle dataset with 
Hosted in AWS, 

## Modeling Steps   

* Transfer Learning:

1. Retrieved all the skill sets related information and counted how frequently each skill appears in the job description(e.g., Python, R).
2. Retrieved sentences which mentioned "year...experience". From there, got the required number of years of experience.
3. Remove all the non-alphabetic characters and stop words. Change the text to lower case. 
3. Remove company names from the job description.
4. Remove common words especially for the ones in section where employers talk about being an equal opportunity employer.
5. Use TF-IDF 2-3 ngrams to tokenized the job description cleaned by the previous two steps.

* Topic Modeling:

1. Initially I was having trouble identifying clear topics. When I used LSA to split the full dataset sets into two topics. I found one is related to medical laboratory research, while the other one is more data science related. Below shows the scatter plot with x & y as the two LSA topic probabilities. Therefore I removed the datapoints related to medical laboratory research (around 100 datapoints). After that, the topic modeling become more clear. 


2. I tried a few techniques include LDA, LSA and NMF. And the one give me the best result is 4-topic-split using NMF. Below I have created a Tableau story book showing the results of exploration data analysis and topic modeling. 
 
## Project Presentaton Slides
<iframe
src="https://docs.google.com/presentation/d/e/2PACX-1vTOdikurq40w-BGsprz3WG3M3OHa9FKh9GlJljHdHeRAYlh8XnTkk7JaGUzTx-KYTDD6UEBkGzOZPAX/embed?start=true&loop=false&delayms=3000"
frameborder="0" width="480" height="299" allowfullscreen="true"
mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

## Future Works 

In the future, I would like to:
1. Ensemble the NLP and Image models together to improve the classification
   accuracy.
2. Given more time and resource, I would train the model using the whole
   original dataset and predict on more product categories.
