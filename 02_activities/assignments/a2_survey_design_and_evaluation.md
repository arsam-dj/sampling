# Assignment: Questionnaire Design and Sample Evaluation

## Requirements

The goal of this assignment is to practice developing and evaluating sampling materials.

### Part A - Survey Design:

Select one of the scenarios below and design a survey to meet the need(s) outlined in the prompt.

1.	In two to three sentences, describe the purpose of your survey
2.	Describe your target population, sampling frame, sampling units, and overall sampling strategy.
3.	Write a 5-10 question survey to address your chosen scenario below.

##### Scenarios
1.	You work in the Human Resources Department at a large tech company. Over the past few months, the company has been experiencing a high turnover rate across many of its departments, specifically within the entry- and lower-level positions. The company wishes to understand why this turnover is happening, and what changes need to occur to improve employee satisfaction.
2.	You work for a Canadian national political party during a federal election. Throughout the campaign period, your party has seen relatively high approval ratings, but an opposing party is also polling favorably and may still have a chance to win the election. You are one month away from the election and you want to understand what voters want from your party and its leader in order to maintain your lead and eventually win the election.
3.	You are a student researcher in the sociology department at the University of Toronto. You are working on a research project that concerns the relationship between music taste and age. This involves both comparisons between different people of different ages and comparisons of the same individual at different ages during their lifetime. You wish to understand to what extent age influences music taste, specifically as it relates to perceptions of popular music. Your results will be written into an academic paper that you hope to publish.

### Part B - Survey Evaluation:

For the **Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33)**, conducted by Statistics Canada find any and all available documentation for the data gathered and identify and describe the survey features indicated below.

1. Sample type
2. Sample size
3. Target population
4. Sampling frame
5. Survey mode(s) 
6. Timeline
7. Response rate
8. Weights
9. Data processing
10. Cleaning, imputation, etc
11. Sources of error
12. Limitations, known biases, etc
13. Link to documentation and any additional sources used


# Your Changes

## Part A - Survey Design: 

The number of your chosen topic: `1`

Describe the purpose of your survey:
```
The purpose of this survey is to understand why entry- and lower-level positions within a tech company appear to be experiencing higher rates of turnover. The HR department hopes that this survey will give them the tools and insights necessary to improve working conditions for entry-level workers and lowering their rates of turnover. This will also benefit the company by reducing the amount of resources spent on having to frequently hire and train new candidates.
```

Describe your target population, sampling frame, sampling units, and observational units:
```
The target population is all entry-level works at this company. The sampling frame is the subset of workers at this company presented with the survey (this depends on the sampling method chosen). The sampling/observational units are those that respond to the survey.

For this scenario I assume that all departments will have a subset of entry-level workers, so it makes sense to stratify the population by department first, then select entry-level workers at random (stratified random sampling). Entry-level workers can be specifically defined as those working with the company for 1-2 years. The survey will be confidential and anonymous, to ensure that employee answers would not affect their employment status.
```

Your 5-10 question survey:
```
1. How long have you worked at this company?
2. What department are you from?
3. What is your salary range?
4. Are you satisfied with your salary? 0-not satisfied at all, 5-very satisfied
5. In the past year, how would you describe your work-life balance? 0-not good, 5-excellent
6. In the past year, would you say you felt welcome in your department? 0-not at all welcome, 5-very welcome
7. In the past year, how much guidance or training did you receive from senior department members? 0-no guidance at all, 5-lots of guidance
8. Do you have any comments on the culture of your department or suggestions on any changes that should be considered?
9. Do you have any comments or feedback on the guidance or mentorship you have received?
10. Do you have any comments or concerns about any other aspects of working at our company?
```

## Part B - Survey Evaluation:

Identify and describe survey features:

```
1. Sample type: respondents were selected by first mailing a letter to selected households, and then having one randomly selected member from these households (aged 15 or older) complete an online questionnaire. This is a two-stage sampling design where sampling units are households and final stage units are individuals. Stratification was done by province and by geographic regions within each province (the researchers reported 27 different strata).

2. Sample size: the target sample size was 20,000 while the actual number of respondents was 16,149.

3. Target population: Canadians from the ten provinces, aged 15 and above.

4. Sampling frame: the frame consists of households with a telephone number available to Statistics Canada and those on the address register (AR); a list of all dwellings within the ten provinces.

5. Survey mode(s): respondents either filled out an internet questionnaire on their own, or filled one with the assistance of a telephone interviewer.

6. Timeline: conducted from September to December 2018.

7. Response rate: the overall response rate was reported to be 41.9%.

8. Weights: a household weight was calculated and then a person weight using the initial household weight.

9. Data processing: survey responses were electronically recorded for data processing. Researchers describe coding most responses (including write-in questions) if possible. Coding followed standard classification systems used by Statistics Canada and conventions followed by other relevant entities like International Classification of Nonprofit Organizations.

10. Cleaning, imputation, etc: duplicate records, non-response, and out-of-scope records were dropped before further processing. If any respondents did not answer the minimum number of questions, their records were dropped as well. Some missing records were imputed using information from elsewhere in the survey if possible.

11. Sources of error: non-sampling errors can arise from interviewers misunderstanding instructions, respondents misunderstanding questions, transcriptional errors, and processing errors. Sampling errors arise from variability from sample responses and a number of statistical tests (eg., confidence intervals) to estimate how well the sample represented the true population.

12. Limitations, known biases, etc: limitations and biases were not explicitly mentioned in the User Guide. I would theorize that some bias would arise from the nature of respondents; those more likely to take the time and respond to this survey would also be more likely to be the giving/volunteering/participating type. 

13. Link to documentation and any additional sources used: I used the User Guide included in the dataset from abacus: https://abacus.library.ubc.ca/dataset.xhtml?persistentId=hdl:11272.1/AB2/GBFDYG

```

## Rubric

-	All required components are present and complete **Complete / Incomplete**
-	Choice of sampling strategy for Part A is justified and related to survey purpose **Complete / Incomplete**
-	Information for Part B is complete and correct **Complete / Incomplete**

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 18/04/2025`
* The branch name for your repo should be: `assignment-2`
* What to submit for this assignment:
    * This markdown file (a2_survey_design_and_evaluation.md) should be populated and should be the only change in your pull request.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sampling/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-2`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via the help channel in Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
