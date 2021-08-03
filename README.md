# Customer Segments [Unsupervised Machine Learning]

This final project in the Unsupervised Learning section, is part of Udacity's Machine Learning Nanodegree program.
I have enjoyed working on it and learned a lot :)

## Project Overview
In this project, I applied unsupervised learning techniques to identify segments of the population that form the core customer base for a mail-order sales company in Germany. These segments I used to direct marketing campaigns towards audiences that will have the highest expected rate of returns.
I used K-means to the general population into clusters, then I used those clusters to see which of them comprise the main user base for the company.
In addition, the dataset in this project required several assessment and cleaning steps before I applied K-means. The ability to perform data wrangling and the ability to make decisions on data were both valuable skills that I practiced in this project.
#### Project Details
Step 0: The Data

I worked with real-life data provided by Bertelsmann partners AZ Direct and Arvato Finance Solution. The data here concerns a company that performs mail-order sales in Germany.
-	Udacity_AZDIAS_Subset.csv: Demographic data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
-	Udacity_CUSTOMERS_Subset.csv: Demographic data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
-	Data_Dictionary.md: Information file about the features in the provided datasets.
-	AZDIAS_Feature_Summary.csv: Summary of feature attributes for demographic data.
-	Identify_Customer_Segments.ipynb: Jupyter Notebook divided into sections and guidelines for completing the project. 

Step 1: Preprocessing

When you start an analysis, you must first explore and understand the data that you are working with. In this (and the next) step of the project, I worked with the general demographics data. The key points were:
-	How are missing or unknown values encoded in the data? Are there certain features (columns) that should be removed from the analysis because of missing data? Are there certain data points (rows) that should be treated separately from the rest?
-	Consider the level of measurement for each feature in the dataset (e.g. categorical, ordinal, numeric). What assumptions must be made in order to use each feature in the final analysis? Are there features that need to be re-encoded before they can be used? Are there additional features that can be dropped at this stage?
I created a cleaning procedure that I applied first to the general demographic data, then later to the customers data.

Step 2: Feature Transformation

At this step, the data is clean, so used dimensionality reduction techniques to identify relationships between variables in the dataset, resulting in the creation of a new set of variables that account for those correlations. In this stage of the project, I attended to the following points:
-	The first technique is feature scaling. 
-	Once I have scaled the features, I applied principal component analysis (PCA) to find the vectors of maximal variability. How much variability in the data does each principal component capture? Can you interpret associations between original features in your dataset based on the weights given on the strongest components? How many components will you keep as part of the dimensionality reduction process?

Step 3: Clustering
Finally, I applied clustering techniques to identify groups in the general demographic data. Then applied the same clustering model to the customers dataset to see how market segments differ between the general population and the mail-order sales company. I tackled the following points in this stage:
-	Use the k-means method to cluster the demographic data into groups. How should you make a decision on how many clusters to use?
-	Apply the techniques and models that you fit on the demographic data to the customers data: data cleaning, feature scaling, PCA, and k-means clustering. Compare the distribution of people by cluster for the customer data to that of the general population. Can you say anything about which types of people are likely consumers for the mail-order sales company?


## Software and Libraries
This project uses Python 3 and is designed to be completed through the Jupyter Notebooks IDE. It is highly recommended that you use the Anaconda distribution to install Python, since the distribution includes all necessary Python libraries as well as Jupyter Notebooks. The following libraries are expected to be used in this project:
•	NumPy
•	pandas
•	Sklearn / scikit-learn
•	Matplotlib (for data visualization)
•	Seaborn (for data visualization)


## Run

In a terminal or command window, navigate to the top-level project directory (where you save it) and run one of the following commands:

```bash
ipython notebook Identify_Customer_Segments.ipynb

```  
or
```bash
jupyter notebook Identify_Customer_Segments.ipynb

```

This will open the iPython Notebook software and project file in your browser.

