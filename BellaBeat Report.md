# BellaBeat Report
## Background
Urška Sršen and Sando Mur founded Bellabeat, a high-tech company that manufactures health-focused smart products. Sršen used her background as an artist to develop beautifully designed technology that informs and inspires women around the world. Collecting data on activity, sleep, stress, and reproductive health has allowed Bellabeat to empower women with knowledge about their own health and habits. Since it was founded in 2013, Bellabeat has grown rapidly and quickly positioned itself as a tech-driven wellness company for women. By 2016, Bellabeat had opened offices around the world and launched multiple products. Bellabeat products became available through a growing number of online retailers in addition to their own e-commerce channel on their website. The company has invested in traditional advertising media, such as radio, out-of-home billboards, print, and television, but focuses on digital marketing extensively. Bellabeat invests year-round in Google Search, maintaining active Facebook and Instagram pages, and consistently engages consumers on Twitter. Additionally, Bellabeat runs video ads on Youtube and display ads on the Google Display Network to support campaigns around key marketing dates. Sršen knows that an analysis of Bellabeat’s available consumer data would reveal more opportunities for growth. She has asked the marketing analytics team to focus on a Bellabeat product and analyze smart device usage data in order to gain insight into how people are already using their smart devices. Then, using this information, she would like high-level recommendations for how these trends can inform Bellabeat marketing strategy.
Ask Phase: Customers usage of non-Bellabeat smart devices to identify trends that could be used to optimize the marketing strategy
## Select one BellaBeat product to apply these insights
Selected the IVY bracelet Designed as an elegant bracelet that monitors your heart rate, respiratory rate, and cardiac coherence, and physical and mental activity, Ivy is a one-of-a-kind health and wellness tracker created for women, by women.
## NB
I am looking for trends in the smart device market that we can use to target customers.
Using these trends, we will be able to know our target audience and how to advertise to them.
Data is span over two months
24 participants for sleep daily
8 participants for weight loss
17 participants at different times did not activate their fitbit devices (Automatically turns on when it notices someone is doing an activity)
## Description of Datasets used
This dataset generated by respondents to a distributed survey via Amazon Mechanical Turk over the span of two months. Thirty-three eligible Fitbit users consented to the submission of personal tracker data, including minute-level output for physical activity, heart rate, and sleep monitoring. Individual reports can be parsed by export session ID (column A) or timestamp (column B). Variation between output represents use of different types of Fitbit trackers and individual tracking behaviors / preferences.
## Cleaning and manipulation of data
1)	Addition of 'VeryActiveMinutes'+'FairlyActiveMinutes'+'LightlyActiveMinutes' to create a new column ‘TotalActiveMinutes’, in the dailymerged csv file.
2)	Creating a new dataset containing the following column; 'Id', 'TotalSteps', 'TotalDistance','Calories','ActiveDate','TotalActiveMinutes','SedentaryMinutes' and saving it as another csv file named dailymerged_new.
3)	Separated the ActivityHour into two different columns for Date and Hour, in the hourlycalories and hourlysteps dataset.
4)	Concatenated the hourlystpes and hourlycalories into a single dataframe for better visualization and saved it as a new csv file new_data.
5)	Created a new column called TimeSpentInBed by subtracting TotalTimeInBed by TotalMinuteAsleep.
## Summary of Analysis
1)	A linear correlation between the TotalDistance and Calories which tells us that the more the users covered the more calories they burned.
2)	Users showed a steady activity usage from 12:00pm to 2:00pm and a major drop around 3:00pm then gradually gained activity from 4:00pm to 6:00pm followed by a drastic drop in activity at 7:00pm.
3)	Users showed a steady burn in calories from 11:00pm while showing very little activity cause most users go to bed.
4)	Tuesdays, Wednesdays and Thursdays are the highest recorded days that users performed more activities and it shows a steady activity usage from Fridays till Mondays (where I assume most users use that as a form of recovery).
5)	Most users have an activity spike at 6:00am showing that’s when most users wake up.
## Key Findings
1)	The most active time women do the most activity(workout) is around 4:00pm to 6:00pm I am guessing after a day at work.
2)	Women do the most activities Tuesdays through Thursdays.
3)	Women average a total of 40 minutes staying in bed after waking up

## High-Level Content Recommendations
I would recommend a software update into the IVY bracelet to automatically turn on when it notices someone is doing an activity, also advertise to women who work 9-5 jobs and women who are starting a working out journey to track their activities and progress.
