# Game-LiveOps-Analyst
A Gaming LiveOps Testing analysis and measure the improvement of Tutorial in-game version 1.6.0 has impacted the User Experience better than in-game version 1.5.2 and decide to roll out 100% Version 1.6.0
# I.Introduction
## 1. Background
1. All users in Russia and using Android devices are playing the game with version 1.5.2.
2. Imagine a LiveOps team member after working on data of game version 1.5.2, found that the tutorial was not good for the user's experience.
3. Hence, the team decided to roll out a new version 1.6.0 to change the Tutorial in-game and you expected this would help increase user experience.
**Special Information:**
The game version 1.6.0 has rolled out 50% since 28-10-2023, meaning 50% of new users will keep playing game version 1.5.2 and 50% of the remaining will play the new version 1.6.0.
You started collecting the data from 28-10-2023 to 10-11-2023 to analyze Data is attached 
https://drive.google.com/file/d/1aNXHaU1iZIrn5siF6i5EwjrxmAkct47d/view

Game version 1.5.2 APK: https://drive.google.com/file/d/1LoLrb0zqS6XnUiMnKyX4cPVnxuTKnbja/view

Game version 1.6.0 APK: https://drive.google.com/file/d/1LxOcYCTGjlWP3xsfLImYxNbYTg-E6ERb/view

## 2. Introduction to Dataset
The data follows the new user - who installed and opened the game for the first time - from 28-10-2023 to 03-11-2023 and follows their activities for the next 7 days.
![image](https://github.com/uyennguyen307/Game-LiveOps-Analyst/assets/162019618/dba7874d-0588-4c70-ac7d-7046195b8b49)

## 3. Business Question
- **Question 1**. How can we know if the improvement of Tutorial in-game version 1.6.0 has impacted the User Experience better than in-game version 1.5.2?
- **Question 2**. Can we roll out 100% game version 1.6.0 to all users or not? Why? (Analyze and evaluate the 2 versions).
- **Question 3**. Based on the data and your experience with the game, do you have any ideas to improve our User Experience? Explain it in detail
(image, text, diagram, logic, game mechanics,...)
# III. Visualization
## 1. Overview
![image](https://github.com/uyennguyen307/Game-LiveOps-Analyst/assets/162019618/a410f6c8-26a2-4551-af3d-b90e6e7e23bc)

## 2. Tutorial Impact
![image](https://github.com/uyennguyen307/Game-LiveOps-Analyst/assets/162019618/b2270a60-5dea-46a4-aff5-7e657d23983b)

## 3. Level churn with each tutorial step
![image](https://github.com/uyennguyen307/Game-LiveOps-Analyst/assets/162019618/3eb98630-f4d7-43d0-8184-d24484911ae6)

## Bonus. Cohort Analyst by Python
**Version 1.5.2:** https://colab.research.google.com/drive/1VSW_kEly0IUNe1BSDAbcHdP87XOkNAfJ#scrollTo=JIunxP4_UqUK

**Version 1.6.0:** https://colab.research.google.com/drive/1Ug0_ibgp9XSbR8czSITYEFLkkcsPL1N1#scrollTo=TUYTT9_WQFh0
# iV. Insight
## Question 1: How can we know if the improvement of Tutorial in-game version 1.6.0 has impacted the User Experience better than in-game version 1.5.2?

We will know the improvement of Tutorial in-game version 1.6.0 has impacted the User Experience better than in-game version 1.5.2 based on the Retention Rate (key metrics) and other metrics that I will show below:

Overall, the number of unique users on Version 1.6.0 is more than on Ver 1.5.2 up to 3.8%. The number of session starts & user engagement on Version 1.6.0 are higher than on Version 1.5.2.at 17.3% and 17.8% respectively

1. In testing 7 days, Version 1.6.0 performed better (Retention Rate by User and User Engagement) than Version 1.5.0. However, both version has the same downtrend 

2. On version 1.5.2, there were up to 98.2% of users participated in the tutorial at level 1 but it's more than 6.51% of users churned at level 1. Meanwhile, version 1.6.0 has Up to 97.9% of users participate in the tutorial process at level 1 but there were 7.22% of users left at level 1 => Even though we have changed the tutorial (added more steps from 6 to 10) to help users, they still have a churn and the churn rate is even higher than before changing from Version 1.5.2

3. The Completed Tutorial rate between the two versions (1.5.2 vs 1.6.0) is not much different at 98.2% and 97.9% respectively

4. The Churn Rate at Easy Level from levels 1 to 20 is still high on both versions (1.5.2 vs 1.6.0), meaning users do not engage with the game if changing the tutorial of version 1.6.0

**Key Finding: The improvement tutorial in-game version 1.6.0 still impacts user engagement but it contributed insignificantly at approximately 2% - 3%**

## Question 2: Can we roll out 100% game version 1.6.0 to all users or not? Why? (Analyze and evaluate the 2 versions)

Based on the data & insight which I have provided, We should not roll out 100% because 
- Tutorial Improvement of Version 1.6.0 has contributed 2% - 3% to User Engagement and Businesses have to pay the hidden cost (employee salaries,...) of releasing a new feature (the improvement of the tutorial)
- _**According to the study of Washington University**_, after testing the Tutorial on three games with varying complexity on over 45000 players, the Department of Computer Science & Engineering claims that “we found that tutorials had a surprisingly negligible effect on player engagement in the game, which are less complex and more similar to other games in their respective genres”

_**Reference the study of Washington University:**_ https://grail.cs.washington.edu/wp-content/uploads/2015/08/andersen2012tio.pdf

## Question 3: Based on the data and your experience with the game, do you have any ideas to improve our User Experience? Explain it in detail (image, text, diagram, logic, game mechanics,...)
There are some ways to increase User Engagement, we have to maintain & uplift User Retention Rate

1. Improve Tutorial more clearance before releasing version 1.6.0 by adding explanation text (number 1 in the picture) in each tutorial step and explaining the button (number 2 in the picture)
  
  ![image](https://github.com/uyennguyen307/Game-LiveOps-Analyst/assets/162019618/5202c68e-cb42-4afa-a480-6e4db3c3ac00)
  
2. Hosting regular events that present unique challenges and reward opportunities and daily challenges. These events bring a sense of freshness and urgency, encouraging people to return to participate

   ![image](https://github.com/uyennguyen307/Game-LiveOps-Analyst/assets/162019618/a9581511-705d-45e5-9d89-1e2e5eedf2c9)

3. Offer limited-time events that offer unique gameplay experiences and reward players with exclusive items. These events serve as an exciting diversion from the main game, injecting a dynamic that keeps them engaged.
4. Seasonal events and tournaments are powerful features, engaging ways to entice players to revisit the game. These events are designed around specific times of the year, holidays, or even global special days.
  + Seasonal events appeal for their novelty, limited availability, and thematic content. These events provide unique challenges and exclusive rewards and feature a game interface makeover.
  + Tournaments can boost player engagement with the competition. It involves leaderboards, offering a platform for players to showcase their skills, compete with others, and earn exclusive rewards. This competitive aspect can drive players to spend more, which leads to higher engagement and retention.

   ![image](https://github.com/uyennguyen307/Game-LiveOps-Analyst/assets/162019618/0395181b-57a2-48b7-a050-954309c6bc6a)




