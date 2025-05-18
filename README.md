<h1>Developing Product Placement Strategies for e-Commerce Using Clickstream Data</h1>

<h2>Abstract</h2>
<h3>Introduction and Literature Review</h3>
This dataset included clickstream data (i.e. the sequence of clicks performed by a user) on an international clothing website based in Poland, from April to August 2008. Łapczyński & Białowąs (2013) collected and analyzed this data via association rule mining and sequence analysis. In this research, the business objective is to create and implement product placement strategies (in terms of page number and location) for the international customers of the online store in order to increase overall profitability and revenue, while the data mining objective is to perform unsupervised machine learning (specifically clustering) on the dataset, in order to understand and analyze the behaviors of customers.

<h3>Methods</h3>
The data was processed by converting the year, month, and day into a binary weekday variable. Countries were grouped based on geographical location, and clicks from Poland and unknown locations were dropped due to dataset imbalance and uninterpretability, respectively. The 14 colors were also regrouped by shade. Columns with high correlation were removed to avoid multicollinearity. Exploratory data analysis was used to visualize trends on clicking location per page, revenue per page, revenue per location and page, and revenue per main category. The Synthetic Minority Oversampling Technique (SMOTe) was used to create a balanced location column. z-score scaling and one-hot encoding were also performed on selected columns. Four clusters were chosen in both the k-means and hierarchical clustering algorithms.

<h3>Results</h3>
Cross tabulations were utilized in comparing the distribution of categorical variables (page number, type of clothing, geographical region, screen location, weekday, and color) in a cluster, while boxplots were used to visualize the distribution of price (the only continuous variable). The k-means algorithm showed more clear-cut results for page numbers and screen locations than the hierarchical clustering algorithm. Cluster 1 in the k-means algorithm generated the most revenue, so salient factors such as page number (1-2, i.e. the early  pages), type of clothing (clothes on sale and blouses), screen location (bottom right), and color (neutral) were identified. However, the distribution of clusters per region is not as clear-cut.

<h3>Conclusion</h3>
Our study conducted customer segmentation to understand customer behavior and recommend personalized produce placement strategies which will contribute to higher revenues. Future work may include other unsupervised machine learning methods, including the number of items purchased per session as a feature, considering purchases in Poland, among others. 

<h2>Files</h2>
<ul>
  <li><code>Slide Deck.pdf</code>: Slide deck used to present the research.</li>
  <li><code>Clickstream Data - Pre-processing and Visualization.ipynb</code>: Codes used to process the data and create relevant visualizations.</li>
  <li><code>Clickstream Data - Machine Leaning.ipynb</code>: Codes used to perform unsupervised machine learning (k-means and hierarchical clustering) on the processed dataset.</li>
  <li><code>colour_names.csv</code>: Auxiliary dataset to convert color codes to colors.</li>
  <li><code>country_names.csv</code>: Auxiliary dataset to convert country codes to countries.</li>
  <li><code>e-shop clothing 2008.csv</code>: Dataset retrieved from <a href="https://archive.ics.uci.edu/dataset/553/clickstream+data+for+online+shopping">UCI Machine Learning Repository</a>.
  <li><code>e-shop clothing 2008 data description.txt</code>: Data dictionary accompanying the above dataset.</li> 
  <li><code>e-shop_processed</code>: Output of the first IPYNB and used in the second IPYNB.</li></ul>

<h2>Credits</h2>
This project was created by Sted Cheng, Annika Montemayor, and Kaitlyn Shu Too, and submitted as a requirement for the course <b>CSCI 113: Business Intelligence</b> taken in the second semester of AY 2023-2024 in Ateneo de Manila University. 


