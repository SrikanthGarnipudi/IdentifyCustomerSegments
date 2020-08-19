# IdentifyCustomerSegments
Udacity nanodegree project to implement using un supervised machine learning techniques

## Table of Contents
Installation
Project Introduction
File Descriptions
After Implementation
Licensing, Authors, and Acknowledgements

## Installation
The following libraries are expected to be used in this project:

- NumPy

- pandas

- Sklearn / scikit-learn

- Matplotlib (for data visualization)

- Seaborn (for data visualization) The code should run with no issues using Python versions 3.*.

## Project Introduction

Using unsupervised learning techniques to identify segments of the population that form the core customer base for a mail-order sales company in Germany. These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of returns. The data that you will use has been provided by our partners at Bertelsmann Arvato Analytics, and represents a real-life data science task.
 
## File Descriptions

Data_Dictionary.md: Information file about the features in the provided datasets.

Identify_Customer_Segments.ipynb: Jupyter Notebook divided into sections and guidelines for completing the project. The notebook provides more details and tips than the outline given here.

## After Implementation

After performing Dimensionality Reduction using PCA, 28 features retained and we can explain over 85% of the variability.

In the first principal components, we know that Number of family houses in the PLZ8 region are very important features PLZ8_ANTG3 & PLZ8_ANTG4 (positive), PLZ8_ANTG1 (negative) top 5 positive and top 5 negative

In the second principal components, we know that Personality typology is a influent factor: event-oriented(+ve), sensual-minded(+ve), dutiful(-ve), religious(-ve) are all in top 5 +ve and top5 -ve

In the third principal components, we know that another personality typology contributes a lot: +ve: dreamful, socially-minded, cultural-minded, family-minded -ve: event-oriented, critical-minded, dominant-minded, combative attitude

To apply clustering to the general population using KMeans, we decided to use 8 clusters to segment the population, because, from the curve of the average distance to centroid, we found that the elbow of the curve is around 8, which is also the turning point of the curve.

We can describe segments of the population that are relatively popular with the mail-order company, and relatively unpopular with the company.

These segments are relatively popular with company: 3 are much more than the public 3 - related high affinity of combative attitude, male, low financial interest

These segments are relatively unpopular with company: 5,6 are much less than the public 5 is mostly related with Personality typology especially low affinity of rational, and relative young age (ALTERSKATEGORIE_GROB) 6 is mostly related with Personality typology especially rational, and high financial interest

## Licensing, Authors, and Acknowledgements

Must give credit to Arvato for the data and udacity for providing this project as part of Nano degree program.
