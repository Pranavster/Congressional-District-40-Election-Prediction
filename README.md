# California-Congressional-District-40-Election-Prediction-Model
Contains exploratory data analysis on congressional general elections in California Congressional District 40 and voter and presidential turnout prediction for 2024
# Congressional District 40
Congressional District 40, currently located in the San Bernardino, Riverside, and Orange counties, had approximately 754 thousand people with the median age of 42.4 and the median household income of $132,031 as of 2023. This district also has a 6.74% increase in poverty rate, and a $933k median property value. The largest industries in Congressional District 40 include healthcare & social assistance, with about 47,000 people, professional, scientific, and technical services, with about 45,800 people and manufacturing, with about 40,800 people.

Founded in 1970, this district was redistributed between various counties throughout its history, from being part of the San Bernardino, Inyo, San Diego, and Orange counties in 2000 to being part of the Riverside and San Bernardino counties in 2024.

Young Kim is the current US representative and the current senators are Alex Padilla and Adam Schiff.

# Objective
The objective of this project was to predict the results of the presidential election results by party, which was correctly predicted to be Kamala Harris. Additionally, the results of the congressional elections and racial breakdown of the results of general elections were also analyzed.

# Analysis of Results
![cbffcc56-3526-447e-ae03-c0853ec61610](https://github.com/user-attachments/assets/7576ffa6-cf8c-4049-8147-d6770d9a3e12)

Based on the sklearn module LogisticRegression, we were able to predict the presidential election results for the 2024 general election.

Given that the results were impacted by the shifting boundaries of California Congressional District, the votes in San Bernardino, Orange, and Riverside counties were counted and the percentage differential was calculated
+---------------+--------------------+--------------------------------------------------------------+--------------+
| Party         |   Predicted Result |   Results for San Bernardino, Orange, and Riverside Counties |   Difference |
+===============+====================+--------------------------------------------------------------+==============+
| Democrat      |        1.79821e+06 |                                                  1.55717e+06 |    15.4795   |
+---------------+--------------------+--------------------------------------------------------------+--------------+
| Republican    |        1.4919e+06  |                                                  1.49698e+06 |     0.339217 |
+---------------+--------------------+--------------------------------------------------------------+--------------+
| Other Parties |    70292           |                                              91341           |    23.0444   |
+---------------+--------------------+--------------------------------------------------------------+--------------+

There were more predicted Democratic voters than actual Democratic voters in the San Bernardino, Orange, and Riverside Counties, and there were more Republican voters in San Bernardino, Orange, and Riverside Counties than what was predicted. There were also more voters for other parties in the San Bernardino, Orange, and Riverside Counties than predicted. The reason for the high percentage error for other parties may have to do with a desire for significant change in policy. The lowest percent error was in the Republican party as the counties which vote Republican haven less population than the ones who vote Democrat. The Democratic percent error can be attributed to the Democratic Orange County having more a higher population than the San Bernardino and Riverside counties. Kamala Harris was predicted to win in California Congressional District 40, which she won in. 

# Room For Improvement
Although many voters in the 2024 presidential election in CA40 voted for Kamala Harris, the candidate of the Democratic party, it does not reflect the actual amount of presidential votes in CA40. This is because the Orange, San Bernardino, and Riverside counties do not exactly correlate with the actual boundaries of the 40th Congressional District, meaning the total number of votes for all the counties in CA40 will likely exceed the amount of votes in CA40. This model could be expanded on by giving a breakdown of votes by socioeconomic class and race, as well as consider the migration in and out of this district.
