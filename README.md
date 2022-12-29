# US Medical Insurance Project
 
In this Python data analysis project, I wanted to demonstrate the various skills I have learned while progressing through the Codecademy Data Science: Analytics Specialist Career Path. At the time of this project, I had not learned about data structures like `pandas` or any of the graphical packages available in `matplotlib`.

## Introduction

In this project, I worked with medical insurance data from the `insurance.csv` dataset. I started by looking through the data to see if it was complete, what types of variables I would be working with, and start asking questions. After reading in the **CSV** file into Python, it revealed that each patient had seven different attributes . . .

* Age (discrete quantitative)
* Sex (qualitative)
* BMI (continuous quantitative)
* Number of Children (discrete quantitative)
* Smoker (qualitative)
* US Geographical Region (qualitative)
* Annual Medical Costs (continuous quantitative)

The dataset appeared to be clean and complete, with every patient attribute containing a value without any inconsistencies to address. The basic questions I asked first included . . .

* What is the average age, BMI, number of children, medical costs of the patients in the sample?
* Is there any skew to the distribution of the data?
* How are the patients distributed amongst the categories?
	* How many males and females are in the sample?
	* How many smokers and non-smokers are there?
	* Are the patients evenly distributed throughout the US geographical regions?

## Analysis

From the initial analysis, percentage of males and females in the sample were approximately equal (50.52% to 49.48%, respectively). The number of non-smokers was a little more than 75% of the entire sample. The patients sprawl across 4 general US geographical regions (Northeast, Southeast, Southwest, and Northwest) with the distribution of the 4 regions being roughly equal.

I calculated both the averages and medians of the ages, number of children, BMI, and annual medical costs. For the variables age, number of children, and BMI, the average and median were approximately equal, indicating that the distribution is roughly symmetric. However, the average cost was much greater than the median cost, indicating a skew of the data to thr right. The average annual cost was also rather large to me ($13,270.42), so I became curious as to what might have cause that rather large skew to such a high average price.

The two factors that immediately jumped out as being key contributors to high medical costs were BMI and Smoking. I wanted to dig deeper into those two variables to see how those two categories influence a patient's annual medical costs. This initial analysis lead me to dig a little deeper into the categories and how they influence the annual cost. The difference in annual cost between the obese and non-obese was $4,836.60. The difference in annual cost between the smokers and non-smokers was $23,615.96. The latter of the findings seemed to suggest that a patient's smoker status contributes rather significantly to their annual medical costs.

More analysis was conducted on average annual cost between males and females and the four geographical regions. The sexes had similar average costs, with males having about $1,000 more in annual costs. The regions paid roughly the same amount per year, with the Southeast having the highest. The Southeast did show a greater difference between the average and median, which lead to exploring each region's average BMI and smoker status. The Southeast averaged the highest BMI (33.36), which is bordering on the morbidly obese boundary, and had the most smokers in the sample (91). These factors likely contributed to the region's higher average and the skew in their average annual costs.

## Conclusion

The findings seem to suggest that a patient's smoker status is a strong contributor to their annual medical costs. The 274 smokers in the sample averaged $32,050.23 per year in medical costs, versus $8434.27 for the 1064 non-smokers in the sample. The amounts to almost $24,000 in potential savings from quitting smoking. These findings could be used in bolstering a campaign to help smokers begin to quit.


