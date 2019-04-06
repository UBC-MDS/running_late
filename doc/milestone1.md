## Running Late - Proposal

|Name|Github |
|---|---|
| Alycia Butterworth | [alyciakb](https://github.com/alyciakb) |
| Sreya Guha | [sreyaguha](https://github.com/sreyaguha) |
| Fan Nie | [Jamienie](https://github.com/Jamienie) |
| Aaron Quinton | [aaronquinton](https://github.com/aaronquinton) |

## Background

When students come to class late, it can disrupt the flow of a lecture or discussion, distract other students, impede learning, and generally erode class morale. At its most extreme, teachers may have to start class 5-10 minutes late in order to account for late arrivals, which means that students will miss out on valuable instructional time on a daily basis. There are a number of possible reasons students arrive to class late. For example, going to bed late and waking up late next morning, an inherent anxiety level associated with attending school. Inevitable circumstances along a student's way to school can also be one of the possible reasons why students are late to class.
In some instances, a student may find it difficult to make it to class on time because of the physical distance between the student's home and school. This may be particularly true of students who live off-campus. Thus explaining our question of interest.

## Question of Interest

The focus of this experiment is to investigate the relationship between commute time and late arrival time. In particular, a survey will be conducted on the 2018-2019 cohort of Masters of Data Science (MDS) students at the University of British Columbia (UBC).  The goal of this experiment is to address the specific question:  **Does the commute time to UBC of a MDS student influence their late arrival time to the first class?**

To uncover the question of interest the following questions will be included in our survey:
- What is your average commute time to the University of British Columbia? - (numerical input)
- During Blocks 1 through 6, what percentage of classes have you arrived late? - (numerical input)
- If you answered a number greater than 0%, for the days you were late, what was the average time (in minutes) that you were late? - (numerical input)

To handle potential confounding variables the survey will include these additional questions:
- What method of transportation do you use? - (transit, bike, walk, drive)
- Do you live on or off campus? - (On Campus, Off Campus)
- Do you consider your self a Morning Person or Night Owl? - (Morning Person, Night Owl)
- How much sleep (in hours) do you get on an average night? - (numerical input)
- Do you work part time? (Yes, No)
- Are you involved in any clubs or extracurriculars? (Yes, No)
- Do you have breakfast/coffee at home, buy on campus, or neither? (At Home, On Campus, Neither)
- How well do you perceive your performance in this program - (Below Average, Average, Above Average, Prefer not to Say)
- Do you live with a partner/family/dog - (Yes, No)

## Analysis

We are planning to use a two-tailed hypotheses test to quantify whether length of commute will influence when MDS students arrive for their first class.
The null hypothesis will be “the length of commute does not influence when MDS students arrive for their first class”. The alternative hypothesis will be “yes, the length of commute does influence when MDS students arrive for their first class”.

The study is observational in nature and will only address the association between commute time and arrival time. Moreover, the data considered is focused on MDS students and is not generalizable to a larger population.  

## Ethical Considerations

The main ethical considerations that pertain to our study, as described in the [UBC Office of Research Ethics document on Using Online Surveys](https://ethics.research.ubc.ca/sites/ore.ubc.ca/files/documents/Online_Survey-GN.pdf), is related to the online survey tool we are using. To fully comply with BC FIPPA, we will be using the UBC-hosted version of Qualtrics to collect our survey responses. This way we can ensure privacy because the results are secured, stored in Canada, and anonymity is preserved by not tracking IP addresses. Our second ethical concern is regarding the question "What is your average commute time to the University of British Columbia?". We have designed it to be a continuous variable and recognize there may be some outliers (e.g. an individual with an extra long commute time) that, when combined with outside information, may create an opportunity to identify an individual. Once we have collected and reviewed our data, we will either removed outlier(s) or perform binning to achieve k-anonymity and ensure the privacy of the surveyed subjects. We have designed many of our survey questions to be categorical to automatically group subjects (minimizing the risk of outliers) and will verify k-anonymity of the categorical variables after data collection.
