# ASSIGNMENT: Sampling and Reproducibility in Python

Read the blog post [Contact tracing can give a biased sample of COVID-19 cases](https://andrewwhitby.com/2020/11/24/contact-tracing-biased/) by Andrew Whitby to understand the context and motivation behind the simulation model we will be examining.

Examine the code in `whitby_covid_tracing.py`. Identify all stages at which sampling is occurring in the model. Describe in words the sampling procedure, referencing the functions used, sample size, sampling frame, any underlying distributions involved, and how these relate to the procedure outlined in the blog post.

Run the Python script file called whitby_covid_tracing.py as is and compare the results to the graphs in the original blog post. Does this code appear to reproduce the graphs from the original blog post?

Modify the number of repetitions in the simulation to 100 (from the original 1000). Run the script multiple times and observe the outputted graphs. Comment on the reproducibility of the results.

Alter the code so that it is reproducible. Describe the changes you made to the code and how they affected the reproducibility of the script file. The output does not need to match Whitby’s original blogpost/graphs, it just needs to produce the same output when run multiple times

# Author: Alex Daiejavad

```
1. Identify all stages at which sampling is occurring in the model.

    i) when a subset of people are randomly infected based on ATTACK_RATE (10% of all people set as default)
        The sample size is 10% of the original population (so, 100/1000 got infected). The sampling frame would be these 100 people. The chance of any person being infected is 10%. The function used is np.random.choice, which simply picks a determined number of cases out of a given population.
    
    ii) when a random subset of the infected are traced (20% of infected set as default)
        The sampling frame are individuals who have been infected (100 individuals as determined in the previous stage). The sample size is 20% of these 100 people (so, 20 individuals) who are then selected for contact tracing. Just like before, any infected individual has a 20% chance of being traced. The function used is np.random.rand, which generates a 1D array of desired n length (100 in this case), where numbers range from 0 to 1. In this case, indexes less than TRACE_SUCCESS were chosen to be infected individuals traced. This time, the number of traced individuals can vary between runs.

2. Run the Python script file called whitby_covid_tracing.py as is and compare the results to the graphs in the original blog post. Does this code appear to reproduce the graphs from the original blog post?

   No, in the blog post, the observed proportion is centered around 0.5 while the true proportion is centered on 0.2. When I run the code, both true and observed proportions are centered around 0.2.

3. Modify the number of repetitions in the simulation to 100 (from the original 1000). Run the script multiple times and observe the outputted graphs. Comment on the reproducibility of the results.

    The graphs are generally reproducible, with both distributions centered somewhere around 0.2 every time.

4. Alter the code so that it is reproducible. Describe the changes you made to the code and how they affected the reproducibility of the script file. The output does not need to match Whitby’s original blogpost/graphs, it just needs to produce the same output when run multiple times

The issue with the original code was that both weddings were combined into a single wedding, and all 80 brunches were combined into a single brunch event. To correct for this, I differentiated wedding1 and wedding2 with 100 attendants each, as well as each of the 80 brunches with 10 attendants each. Running the code confirms that the two distributions are no longer similar to one another; the observed proportion is now centered further to the right relative to the true proportion.
```


## Criteria

|Criteria|Complete|Incomplete|
|--------|----|----|
|Altercation of the code|The code changes made, made it reproducible.|The code is still not reproducible.|
|Description of changes|The author explained the reasonings for the changes made well.|The author did not explain the reasonings for the changes made well.|

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 09/04/2025`
* The branch name for your repo should be: `assignment-1`
* What to submit for this assignment:
    * This markdown file (a1_sampling_and_reproducibility.md) should be populated.
    * The `whitby_covid_tracing.py` should be changed.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sampling/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-1`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via the help channel in Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
