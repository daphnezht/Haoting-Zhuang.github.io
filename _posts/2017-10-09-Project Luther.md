---
layout: post
title: Greater Seattle House Price & Appreciation
---
The second project is about applying the knowledge that we learned about linear regression. 

###Why this topic?
My husband and I recently moved to Seattle. Last year, when we started to
search for our new home, we had a hard time comparing different properties and
decide how high we should reasonably go for a offer in this competitive
market. Also,as you could see from below chart which shows the annual
percentage increase of median house price, Seattle area has become one of the
fastest appreciating metro areas among the nation. There could be good
opportunites for real estate investors.  These drive me to create a model that
could predict property price/appreciation which would help home buyers and
investor make better decisions. 

![](/images/Redfin_chart.png?raw=true) 

### Data Source and size

Using selenium and beautiful soup, I scraped my data from www.redfin.com for all properties sold in the past 3
months in the city of n Seattle, Kirkland, Bellevue and Redmond.
   
* Data Size:
   * 4290 data points (Price)
   * 2895 data points (Annual Appreciation)
 
* Features:
   * 8 Numeric ones:$/Square feet, # of Baths,  # of Beds, HOA/Month, Square
     feet, School Avg Rating, Year Built, Lot size   
   * 2 Categorical ones: Property Type,  Zip Code

### Modeling steps

1. Eliminate outliers & transform skewed data
2. Standardized numeric features
3. Generate dummy variables for categorical features
4. Perform k fold cross validation and select key features based on p values
5. Increase polynomial degree of the key features
6. Use cross validation to determine the ideal alpha value in regulation tool
(Lasso, Ridge) to minimize test error

### Results and findings


![](/images/Top&BottomZip.png?raw=true)

### Additional Works
For future works, I would like to first further refine my model by collecting
more data and identify more featues. 
Second, I would like to perform renting vs buying benefit analysis and ROI
(return on investment) so that home buyer/investor can easily compare two properties in terms of their financial values. In order to do that, I will incorporate renting information (e.g., average rent in the
closeby area), mortgage rate, tax, maintenance expense into consideration.

### Leasons Learned
I have learned a lot throughout this process.There's been road blocks and
several back and forths. 
Here's some of big take-aways. 
* Explore more data sources early on:
 
* It's better to scrape more, rather than less, data than you need:
     For this porject, opening up 4000+ pages to scrape the data scraping could take a full day or longer.
* Add time delay and error handling exception while doing data scraping:
 
* Create functions to make the code clean:

* Don't give up too early


