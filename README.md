# Running Late

| Contributors | Github |
|--------------|--------|
| Alycia Butterworth | [alyciakb](https://github.com/alyciakb) |
| Sreya Guha | [sreyaguha](https://github.com/sreyaguha) |
| Fan Nie | [Jamienie](https://github.com/Jamienie) |
| Aaron Quinton | [aaronquinton](https://github.com/aaronquinton) |


## Overview

Below is a brief introduction and overview to our project. For the detailed report and analysis, [please click here.](https://github.com/UBC-MDS/running_late/blob/master/doc/final_report.md)

### Introduction


When students come to class late, it can disrupt the flow of a lecture or discussion, distract other students, impede learning, and generally erode class morale. At its most extreme, teachers may have to start class 5-10 minutes late in order to account for late arrivals, which means that students will miss out on valuable instructional time on a daily basis. The focus of this experiment is to investigate the relationship between commute time and late arrival time. In particular, a survey will be conducted on the 2018-2019 cohort of Masters of Data Science (MDS) students at the University of British Columbia (UBC). 

The goal is to address the specific question: **Does the commute time to UBC of an MDS student influence their arrival time to the first class?**

- *Null Hypothesis:* Commute time to UBC does NOT impact an MDS student's late arrival time to class.
- *Alternative Hypothesis:* Commute time to UBC does impact an MDS student's late arrival time to class.

### Survey Design

To address this question we surveyed students in the 2018-2019 MDS cohort to obtain data to conduct our analysis. We used the services provided by Qualtrics to make our survey. We provided a consent form to disclose the potential risk of re-identification of the anonymous data when combining with application information in the MDS program. The survey can be found here: [Running Late Survey](https://ubc.ca1.qualtrics.com/jfe/form/SV_3Jk3TZyscxiUZY9).

### Data Variables

Our data variables are described below. The full data set can be found in [data/clean_survey_data.csv](https://github.com/UBC-MDS/running_late/blob/master/data/clean_survey_data.csv).

| Variable Name | Type | Description                                    |
|---------------|------|------------------------------------------------|
|`ave_late` | continuous | The multiplied value of percentage of classes the respondent arrived late by the average time in minutes that they were late |
|`Q2.commute_time`| continuous | The respondent's commute time to UBC in minutes |
`Q5.transport` | categorical | The respondent's most used method of transportation for commuting to school |
|`Q6.campus` | binary | Whether the respondent lives 'on campus' or 'off campus' |
| `Q7.sleep_type`| categorical | Does the respondent classify themselves as a 'morning person', 'night owl', or 'neither' |
|`Q8.sleep_time` | continuous | How much sleep the respondent gets on an average night |
|`Q9.work`| binary | Does the respondent works part-time/full-time |
| `Q10.clubs` | binary | Is the respondent a member of any clubs or extracurriculars |
| `Q11.breakfast` | categorical | Does the respondent eat/get breakfast/coffee in the morning 'at home', 'on campus', or 'neither' |
|`Q12.performance`| categorical | How does the respondent perceive their performance in MDS |
|`Q13.family` | binary | Does the respondent live with a significant other, child(ren), and/or dog(s) |

### Exploratory Data Analysis

Our exploratory data analysis (EDA) can be found in [doc/eda_running_late.md](https://github.com/UBC-MDS/running_late/blob/master/doc/eda_running_late.md).

### Analysis

In our EDA we found our data being highly zero inflated, we decided that to appropriately model this distribution we would need a hurdle model. In this approach, the first model (model 1) is the likelihood a student is late given their commute time. The second model (model 2) only considers the students that arrived late or in other words the students that have surpassed the hurdle.

The full analysis can be found in [doc/final_report.md](https://github.com/UBC-MDS/running_late/blob/master/doc/final_report.md).

### Results

In both model 1 and model 2, we did not find sufficient evidence to reject the null hypothesis at a 95% confidence level. Therefore, we have accepted the null and have concluded that there is no relationship between commute time and average minutes late to class.

<br>
<br>
<br>

| Milestone | Version | files and links |
|--------------|--------|------------------------|
| milestone 1 | [V1.0](https://github.com/UBC-MDS/running_late/releases/tag/v1.0) | [Proposal](https://github.com/UBC-MDS/running_late/blob/master/doc/milestone1.md)|
| milestone 2| [V2.0](https://github.com/UBC-MDS/running_late/releases/tag/v2.0) | [EDA](https://github.com/UBC-MDS/running_late/blob/master/doc/eda_running_late.md),  [Survey](https://ubc.ca1.qualtrics.com/jfe/form/SV_3Jk3TZyscxiUZY9),  [Survey Raw Data](https://github.ubc.ca/MDS-2018-19/survey-data/blob/master/2019-04-03_Running_late_survey_data.csv)
| milestone 3 | [V3.0](https://github.com/UBC-MDS/running_late/releases/tag/v3.0) | [Final Report](https://github.com/UBC-MDS/running_late/blob/master/doc/final_report.md), [Peer Review](https://github.com/UBC-MDS/MDS_Block_Difficulty_Perception/issues/16) |

## Code of Conduct

[Our contributor code of conduct can be found here.](https://github.com/UBC-MDS/running_late/blob/master/CONDUCT.md)

## Contributing

[Our contibuting guidelines can be found here.](https://github.com/UBC-MDS/running_late/blob/master/CONTRIBUTING.md)
