# **Which Factors are Most Correlated to Heart Disease?**
## A Project by Samiah Siddiqua
[View my presentation!](https://canva.link/shcmck21e91qyei)
---
### Aiming to discover which factors are most linked to the development of heart disease, this project was presented at University of California, Berkeley, for the Fall 2026 Big Data at Berkeley Bootcamp.

## **Background**

According to the U.S. Centers of Disease Control and Prevention, heart disease is the leading cause of death for men and women worldwide—to put that into perspective, it kills at least one person every 34 seconds.

These statistics make advances in prevention necessary. However, with over 300 factors linked to cardiovascular disease, it is hard to pinpoint what to prevent in the first place. Thus, I decided to research and explore these factors to answer the question, "Which Factors are Most Correlated to Heart Disease?"

Answering this question is important in terms of preventing of cardiovascular disease and the deaths it could cause going forward.

## **The Dataset**
[*Indicators of Heart Disease*](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease), as updated in 2022, contains survey data of over 400,000 Americans in relation to their health and the factors that may or may not lead them to heart disease. 

---

This dataset features rows of patient responses that detail approximately 40 factors, such as whether or not a respondent had depressive disorder.

## **Data Cleaning**
My code will perform cleaning steps such as renaming and unhiding missing columns, dropping unnecessary columns, checking and removing missing or NaN values—since this version of the dataset has NaN values unremoved—and deleting identical columns. Since patient responses are strings by default, I will have them changed to numerical data types using booleans and create binary columns.

It is important to clean this dataset for my project specifically, because I can only use floats and integers to calculate correlation between different factors and heart disease.

## **Finding Correlation**

I have created and concatenated two balanced dataframes—one with a random sample of patients who have heart disease, one with an equal sample of patients who do not—such that this new dataframe has an even amount of people with the disease and people without it. I can then calculate and read a correlation matrix to determine which factors are most likely to cause heart disease.

## **Exploratory Data Analysis**
Three visualizations support an answer to my question.

---

First, a my correlation heatmap shows how certain factors can be correlated to one another and to heart disease. Redder boxes signal stronger correlation in comparison to bluer ones. In terms of my project, the heatmap quickly reveals how angina has the strongest correlation to heart disease out of all other factors. Additionally, age category and difficulty walking also have moderate correlation.

---

Second, a bar plot visualizes one of the strongest uncovered correlations—that of angina's relation to heart disease. It proves that the likelihood of having heart disease increases for patients with angina compared to patients without it.

---

Finally, a line plot displays how as age increases, so does the risk of heart disease—meaning that these two factors may exhibit a direct relationship.

## **Conclusion**
Although the null hypothesis would be that there is no factor correlated to heart disease, a permutation test rejects it and validates the alternative hypothesis of there being, in fact, correlations from certain factors to heart disease. Through this project, I have discovered that angina, age group, and difficulty walking are prominent among other factors in terms of their correlation to cardiovascular disease.
