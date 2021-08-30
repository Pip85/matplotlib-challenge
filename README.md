# **practice-matplotlib**

Student project - analyze datasets on squamous cell carcinoma tumor volumes in mouse studies using Pandas with plots from Matplotlib.  

## **software/tools used**

* pandas:  https://pandas.pydata.org/<br>
  * libraries:<br>
    * Matplotlib.pyplot<br>
    * SciPy stats<br>
* Jupyter Notebook:  https://jupyter.org/<br>


## **resources**
* Background and datasets provided as part of Georgia Tech Data Analytics Boot Camp:<br>
© 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.<br>
* Mouse dataset: <br>
* https://github.com/Pip85/practice-matplotlib/blob/main/Pymaceuticals/data/Mouse_metadata.csv
* Results dataset: <br>
* https://github.com/Pip85/practice-matplotlib/blob/main/Pymaceuticals/data/Study_results.csv

## **project background**

* While your data companions rushed off to jobs in finance and government, you remained adamant that science was the way for you. Staying true to your mission, you've joined Pymaceuticals Inc., a burgeoning pharmaceutical company based out of San Diego. Pymaceuticals specializes in anti-cancer pharmaceuticals. In its most recent efforts, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.<br>

* As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. You have been tasked by the executive team to generate all of the tables and figures needed for the technical report of the study. The executive team also has asked for a top-level summary of the study results.<br>

* Your tasks are to do the following:

  * Before beginning the analysis, check the data for any mouse ID with duplicate time points and remove any data associated with that mouse ID.

  * Use the cleaned data for the remaining steps.

  * Generate a summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.

  * Generate a bar plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the total number of measurements taken for each treatment regimen throughout the course of the study.

  * Generate a pie plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the distribution of female or male mice in the study.

  * Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Calculate the quartiles and IQR and quantitatively determine if there are any potential outliers across all four treatment regimens.

  * Using Matplotlib, generate a box and whisker plot of the final tumor volume for all four treatment regimens and highlight any potential outliers in the plot by changing their color and style.

  * Select a mouse that was treated with Capomulin and generate a line plot of tumor volume vs. time point for that mouse.

  * Generate a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

  * Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment. Plot the linear regression model on top of the previous scatter plot.

  * Look across all previously generated figures and tables and write at least three observations or inferences that can be made from the data. Include these observations at the top of notebook.

## **acknowledgement**

* Background and datasets provided as part of Georgia Tech Data Analytics Boot Camp:<br>
* Mockaroo, LLC. (2021). Realistic Data Generator. [https://www.mockaroo.com/](https://www.mockaroo.com/)<br>
* © 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.

* Project Author:  Valerie Pippenger - https://github.com/Pip85

## **process**

* This challenge included looking at results from mouse studies on squamous cell carcinoma tumor volumes across several drug regimens.  
* The study is sponsored by Pymaceuticals, who is looking at the efficacy of their drug Capomulin.
* The challenge involved cleaning the data for duplicate mouse information.
* A comparison table of statistical measures, mean, median, variance, standard deviation and SEM was prepared using two different coding methods.

![stats](https://github.com/Pip85/practice-matplotlib/blob/main/images/drug_stats.png)

Bar charts comparing total measurements in each of the drug regimens was prepared using two different plotting methods.

**Pandas**
![bar1](https://github.com/Pip85/practice-matplotlib/blob/main/images/drug_measures_bar.png)

**Matplotlib**
![bar2](https://github.com/Pip85/practice-matplotlib/blob/main/images/drug_measures_bar_matplotlib.png)

Pie charts comparing the percentage of female vs male mice were included using two different plotting methods.

**Pandas**
![pie1](https://github.com/Pip85/practice-matplotlib/blob/main/images/gender_pie_pandas.png)

**Matplotlib**
![pie2](https://github.com/Pip85/practice-matplotlib/blob/main/images/gender_pie_matplotlib.png)

* Four promising drug regimens, including Capomulin, were examined using final tumor volume measurements taken over the 45 day study.
* Statistical measures including quartiles, iqr and lower/upper bounds were quantitatively calculated.  Outliers were also revealed in one of the drug regimens, Infubinol.
* Statitical measures and outliers were plotted in a box plot for better visualization.

![box](https://github.com/Pip85/practice-matplotlib/blob/main/images/tumor_volumes_by_drug_boxplot.png)

*One mouse was chosen from the Capomulin and a plot of tumor volume over the 45 day study was created.  While Capomulin seems successful overall, this particular mouse's tumor volume increased over the study.

![line](https://github.com/Pip85/practice-matplotlib/blob/main/images/Capomulin_treatment_linechart.png)

* A scatter plot was generated to show the average tumor volume compared by mouse weight for Capomulin.

![scatter](https://github.com/Pip85/practice-matplotlib/blob/main/images/Capomulin_tumorvol_vs_mouseweight_scatter.png)

* That same scatter plot was regenerated to show the linear regression and the correlation coefficient was calculated.

![regression](https://github.com/Pip85/practice-matplotlib/blob/main/images/Capomulin_tumorvol_vs_mouseweight_regression.png)

* Based on the correlation coefficient and the plotted linear regression equation, there does seem to be a linear correlation between average tumor volume and weight in Capomulin.
