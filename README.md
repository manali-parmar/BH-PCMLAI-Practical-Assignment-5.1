# BH-PCMLAI-Practical-Assignment-5.1
This repository contains code for the practical application assignment 5.1<br>
by Manali Parmar<br>

# Link to the [Notebook] (https://github.com/manali-parmar/BH-PCMLAI-Practical-Assignment-5.1/blob/main/Assignment%205.1.ipynb)

## Summary of Findings:

# Initial dataset related:
1. Explored the dataset to get a general idea of the data elements. File size: Rows 12684 and Columns: 26
2. Investigated dataset for missing data and saw that 99% of the data from 'car' column was missing.
3. Determined to drop the missing data based on % of missing datacells in various columns (very low for other columns with missing data)
4. Calculated acceptance rates from the overall cleaned data and found out that 57% of the drivers accepted the coupons while the remaining 43% did not.
5. Upon plotting the coupon types, the highest category based on coupon count was 'Coffee House' followed by 'Restaurant(<20)', 'Carry out & Take away', 'Bar' and then 'Restaurant(20-50)'.
6. The temperature histogram plot shows the count against various temperature values (highest at 89.5). Also plotted a separate histogram to show the internal distribution of coupons in the overall plot.

# Bar coupon Findings / Actionable insights:
1. Extracted the dataset containing 'Bar' coupons using query method and calculated acceptance rates. Found out that 41% of the drivers accepted the coupons while the remaining 59% did not. Compared to the overall dataset (57%), the acceptance rate for 'Bar' coupon category (41%) is lower.
2. Frequent bar goers have a higher tendency to accept coupons (76%) compared to those who never went or visited less (37%).
3. Upon deeper analysis, found out that the acceptance rate of those who went to a bar more than once a month and are over the age of 25 is 69% while for the remaining others it is significantly low (34%).
4. Acceptance rate of drivers who go to bars more than once a month and had passengers that were not a kid and had occupations other than farming, fishing, or forestry is 70% while for the remaining others is 33% only.
5. These findings help determine the type of population that can be targeted for promotions that will lead to higher probability of acceptance.
6. Based on the data observations, the lower income drivers who frequently visit cheap restaurants are less likely to accept a coupon versus those who are frequent bar visitors under age 30 or frequent bar visitors who are not with kids and have companions. Higher acceptance rates are linked to social commuters and young drivers as they are more likely to accept coupons when they go to a bar frequently.

# Carry out & take away coupon Findings / Actionable insights:
1. About 3/4th of the 'Carry out & Take away' coupons are accepted which is high compared to 'Bar' coupon acceptance rate    of 41%. The below plot provides a general idea of how the data looks with respect to acceptance or not for the 'Carry out    & Take away' coupons dataset.
2. The acceptance rate is highest in the group 'never' versus lowest in the group 'less1' which shows that the drivers are promptly interested to try out new Carry Out & Take Away places for the first time. However, becoming a repeat customer is slightly less likely. The acceptance rates for those with visits more than a month is higher again.
3. Carry out coupons are of high convenience relief for tired drivers who want to pick up dinner on their way back from work without sitting down at a restaurant. So offering coupons in the evening time when drivers are commuting back home will be more efficient.
4. Value for 'toCoupon_GEQ25min' shows positive while 'toCoupon_GEQ15min' displays a negative correlation with acceptance.
5. Rainy or Snowy weather, morning hours when drivers are going to work is not a good choice to promote coupons.
6. Upon exploring the relationship between the expiration and acceptance rates, found out that 1 day coupons have better acceptance rate than 2 hour coupons.
