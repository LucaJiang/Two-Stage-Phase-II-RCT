# Script for presentation

## Introduction: Clinical Trials

A clinical trial is a research study that tests how well new medical treatments work in people. The goal of clinical trials is to determine if a new test or treatment works and is safe.  Here are the three main phases of clinical trials.

According to the FDA, the first phase of clinical trials aims to determine the safety and dosage of the new treatment. This phase typically involves 20-100 healthy volunteers or patients, and has a success rate of approximately 70%.

The second phase of clinical trials aims to determine the efficacy and side effects of the new treatment. This phase typically involves up to several hundred patients, and has a success rate of approximately 33%.

The third phase of clinical trials aims to determine the efficacy and monitor adverse reactions of the new treatment. This phase typically involves 300 to 3,000 patients, and has a success rate of approximately 25%-30%.

## Phase II Clinical Trials

Today, we will focus on the second phase of clinical trials when the endpoint is binary, such as response or no response. In this phase, the objective is to determine if the new treatment is effective enough to warrant further study in a larger phase III trial, as well as to further assess safety. We want to test the hypotheses that the true response rate is greater than or equal to a certain level. Also, we want to control the type I and type II errors at certain levels.

To control the two types of errors, we need a sufficient large sample size. But, it's obviously neither ethical nor practical to enroll an infinite number of patients. So, we need to find a balance between the sample size and the error rates. In this presentation, we will introduce Simon's two-stage optimal design to calculate the sample size.

## A Motivating Example

Here is a motivating example. Suppose we want to test the hypotheses that the true response rate is at least 25% versus at most 5%. We want to control the type I error and type II error at 0.1 each. Also, we want the sample size to be as small as possible.

Let's calculate the sample size under Simon's two-stage optimal design. In this design, we first enroll a small number of patients in stage I. If the number of responses in stage I is greater than a certain threshold, we proceed to stage II. Otherwise, we stop the trial. The sample size in stage II is determined based on the number of responses in stage I.

Here's the flowchart. But, the question is: why do we need a two-stage design? Why not just enroll all patients at once? The calculation result would tell us the anwer.

The result is here and it says that we need to enroll at most 24 patients in total. If we are allowed to stop the trial after stage I, the expected sample size is only 14.5 and the probability of early termination is 0.63. So, the answer is that a two-stage design can save time and resources by stopping the trial early.

## Phase II Clinical Trials

Let's continue to talk about the phase II clinical trials. For sample size calculation, we have two kinds of designs: Optimal designs and Mini-max designs. The optimal designs minimize the expected sample size, while the mini-max designs minimize the maximum sample size. Back to the previous slide, we can see they are different.

## Calculation of Sample Size

The calculation of sample size is based on the binomial distribution. Suppose X1 and X2 are the number of responses in stage I and stage II, respectively. We define the new drug as a failure if the it dose not meet the requirement of stage I which means X1 < R1. Or, it pass the stage I but fail in stage II which means X1 + X2 < R. On the contrary, we define the new drug as a success if it pass both stages.

Therefore, we can relate the probability of failure and success to the type I and type II errors. Also, these probabilities are related to the sample size by the binomial distribution. So, we can calculate the sample size by solving the inequalities.

After that we can calculate the expected sample size and the probability of early termination.

Here's the algorithm to calculate the sample size. First, we set the parameters: p0, p1, alpha, beta and a maximum sample size of searching. Then, we use grid search to find all possible sample sizes. Finally, we calculate the expected sample size and the probability of early termination for each possible sample size.

Here's the result of the algorithm based on our pervious example. The inflection point is all the possible sample sizes. The 'M' stands for minimax design and the 'O' stands for optimal design.

## References

And here are the references. Thank you for your attention.
