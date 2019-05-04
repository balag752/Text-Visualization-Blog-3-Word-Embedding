# Text-Visualization-Blog-3-Word-Embedding



Date: **07.05. (Due: 05.05.)**

Name: **Balaji Subramani**

Session: **[Dimensionality-Reduction](https://textvis.repke.eu/index.html)**

Code: on **[GitHub](https://github.com/balag752/Text-Visualization-Blog-3-Word-Embedding)**

# 

Trip Adviser - Word Embeddings

## Objective

This blog is focused to explore the feature of word embedding techniques using the Trip Adviser hotel reviews. Here we have used word2vec with CBOW (Continuous Bag of Words) and Skip-gram models. we could find more information about this model [here](%5Bhttps://www.kdnuggets.com/2018/04/implementing-deep-learning-methods-feature-engineering-text-data-cbow.html%5D(https://www.kdnuggets.com/2018/04/implementing-deep-learning-methods-feature-engineering-text-data-cbow.html)

## Data Preparation

We have extracted date features (date, month and year) from time of comments updated. As well merged the comments description with each hotel ratings.

## Year wise word similarity

We have online reviews from year 2002 to 2009. Also, at begining of the years, we dont have much reviews. But as time flies, review counts also increased.

It is really interesting to see the evolvement of **cheap** word through out the time. All the periods, it has good connection with expensive and inexpensive words. Also, it has connection with **worse** and **okay** words.

![5cce05faee179](https://i.loli.net/2019/05/05/5cce05faee179.jpg)![5cce05faee179](https://i.loli.net/2019/05/05/5cce05faee179.jpg)

*Interative way of seeing the Report :* **[Tableau Public Yearwise Report](https://public.tableau.com/profile/balag752#!/vizhome/Yearwisewordsynonyms/Yearwisesynonyms)**

We also below depicted **fare** word similarity. Each year it has different similarities. But in whole mostly different sight seeing places and tourist places are related with fare word.

![yearwise fare word](https://i.loli.net/2019/05/05/5cce07e00c437.jpg)![yearwise fare word](https://i.loli.net/2019/05/05/5cce07e00c437.jpg)

*Interative way of seeing the Report :* **[Tableau Public Yearwise Report](https://public.tableau.com/profile/balag752#!/vizhome/Yearwisewordsynonyms/Yearwisesynonyms)**

Above all results are modeled using CBOW.

## Word Similarity in different countries

We have choosed 3 different cities and some important word to compare the each city similarities.

![CBOW Country wise word similarity](https://i.loli.net/2019/05/05/5cce08661c880.jpg)![CBOW Country wise word similarity](https://i.loli.net/2019/05/05/5cce08661c880.jpg)

*Interative way of seeing the Report :* **[Tableau Public Country wise CBOW Report](https://public.tableau.com/profile/balag752#!/vizhome/countrywordusageCBOW/CountrywisewordusageCBOW)**

Above graph is again modeled in CBOW. But below graph is modeled in Skip gram with same word similarity in same 3 cities.

![SG Country word similarity](https://i.loli.net/2019/05/05/5cce08baeabed.jpg)![SG Country word similarity](https://i.loli.net/2019/05/05/5cce08baeabed.jpg)

*Interative way of seeing the Report :* **[Tableau Public Country wise SG Report](https://public.tableau.com/profile/balag752#!/vizhome/countrywordusageSg/CountrywisewordusageSkipgram)**

Both algorithm has different result set. But intuitively Skip gram has more reasonable results as well as **CBOW** has connected with inaccurate words like numbers and stop words.

Also, when training the model Skip gram took more time than CBOW. **Italian foods** are more connected with **food** in New york and London. At the same time, **vegtarian** is connected with food in New delhi. Furthermore, **Flight** is connected with **waited** word in new delhi.

## Low & Top rated Hotel reviews

We also tried to compare the top and low rated hotel reviews. Here green color marks are denoting the 5 star rated hotels and red is pointing to the 1 star rated hotels.

![Rating based results](https://i.loli.net/2019/05/05/5cce0a9bc344e.jpg)![Rating based results](https://i.loli.net/2019/05/05/5cce0a9bc344e.jpg)

*Interative way of seeing the Report :* **[Tableau Public Low & Top Rated Hotel Report](https://public.tableau.com/profile/balag752#!/vizhome/TopLowRatingwordmeanings/Ratings?publish=yes)**

In both top & low rated reviews, **food** is connected with *out*. Notably, **wait** is related with **flight** in low rated reviews and **good** and **excellent** are connected in top rated reviews.
