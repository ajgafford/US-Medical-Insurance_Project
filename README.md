# US Medical Insurance Project
 
In this Python data analysis project, I wanted to demonstrate the various skills I have learned while progressing through the Codecademy Data Science: Analytics Specialist Career Path. 

## Introduction

In this project, I worked with medical insurance data from the `insurance.csv` dataset. I started by looking through the data to see if it was complete, what types of variables I would be working with, and start asking questions. After reading in the **CSV** file into Python, it revealed that each patient had seven different attributes . . .

* Age (discrete quantitative)
* Sex (qualitative)
* BMI (continuous quantitative)
* Number of Children (discrete quantitative)
* Smoker (qualitative)
* US Geographical Region (qualitative)
* Annual Medical Costs (continuous quantitative)

The dataset appeared to be clean and complete, with every patient attribute containing a value without any inconsistencies to address. The basic questions I wanted answered first included . . .

* What is the average age, BMI, number of children, medical costs of the patients in the sample?
* Is there any skew to the distribution of the data?
* How are the patients distributed amongst the categories?
	* How many males and females are in the sample?
	* How many smokers and non-smokers are there?
	* Are the patients evenly distributed throughout the US geographical regions?

## Initial Analysis

From the initial analysis, percentage of males and females in the sample were approximately equal (50.52% to 49.48%, respectively). The number of non-smokers was a little more than 75% of the entire sample. The patients sprawl across 4 general US geographical regions (Northeast, Southeast, Southwest, and Northwest) with the distribution of the 4 regions being roughly equal.

I calculated both the averages and medians of the ages, number of children, BMI, and annual medical costs. For the variables age, number of children, and BMI, the average and median were approximately equal, indicating that the distribution is roughly symmetric. However, the average cost was much greater than the median cost, indicating a skew of the data to thr right. The average annual cost was also rather large to me ($13,270.42), so I became curious as to what might have cause that rather large skew to such a high average price.

The two factors that immediately jumped out as being key contributors to high medical costs were BMI and Smoking. I wanted to dig deeper into those two variables to see how those two categories influence a patient's annual medical costs.