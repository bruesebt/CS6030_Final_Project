# Project Report

### Brad Bruesewitz
### Advanced Software Engineering
### 12/10/2021

## Introduction 
The overarching goal of SURF was to save software developers time and effort when extracting data from user feedback, specifically in app store reviews. Reviews contain vital information, and most developers are not going to spend time sifting through user reviews to obtain information pertaining to their mobile app. There may be a team responsible for interacting with these reviews, but will likely not extract very much useful information from said reviews. SURF seeks to meet this need by extracting information from app store reviews, performing NLP techniques on this extraced information, and outputting a meaningful summary of information contained in the app reviews.

## Problem
The problem with the paper is its evaluation of the tool SURF. The study performed two different experiments, with varying results. One experiment seemed to approve of SURF, and thought that it was useful. THe second experiment on the other hand, seemed to disagree. While 87.50% of the devlopers in Experiment I thought the summaries "Contained no unnecessary information", a meager 28.57% agreed that there was no unnecessary information contained in the summaries in Experiment II. This drastic difference among others prompted me to form my own conclusions based on running the tool myself, collecting data, and evaluating my results in comparison to the results reported in the paper. By reading the paper alone, I found it difficult to form my own opinion on the usefulness of SURF. The paper argues that SURF accomplishes everything it set out to do, but upon reading the paper I was not convinced. I wanted to see the full results myself. My goal for this project was to assess the usefulness of SURF based on the following criteria:
  - Does SURF save me time?
  - Are reviews correctly classified?
  - Does SURF help me better understand user needs?

## Results
I completed all the runs of the XML input and manually read through all the reviews. I identified which ones I believed to be misclassified, out of how many total reviews in the particular category. I compared my results to the results obtained by the study in the paper and this is the comparison table:

|                  | GUI  | APP  | COMPANY | CONTENTS | DOWNLOAD | FEATURE/FUNC. | IMPROVEMENT | MODEL | PRICING | RESOURCES | SECURITY | UPDATE/VERSION | TOTAL |
| ---------------- | ---- | ---- | ------- | -------- | -------- | ------------- | ----------- | ----- | ------- | --------- | -------- | -------------- | ----- |
| Correctness Rate |      |      |         |          |          |               |             |       |         |           |          |                |       |
| Their Experiment | 0.82 | 0.94 | 0.38    | 0.87     | 0.97     | 0.94          | 0.93        | 0.86  | 1.00    | 0.83      | 0.94     | 0.86           | 0.91  |
| My Experiment    | 0.73 | 0.83 | 0.75    | 0.83     | 0.94     | 0.79          | 0.86        | 0.78  | 0.80    | 0.67      | 0.63     | 0.87           | 0.80  |


As you can see, in general my correctness rate was lower in comparison to the results from the experiment in the paper. The only exception would be the "Company" category. I did not agree with all of the misclassifications found in the paper, and there were very few reviews in this category so the few changes led to a drastically different percentage.
