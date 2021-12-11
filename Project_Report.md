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

In addition to assessing the accuracy of the classification functionality, I wanted to see if the tool would be useful in terms of time saving. However, there were multiple components that I thought were missing from the data in the experiments conducted by the paper. I decided to conduct an experiment of my own as a way to see if SURF would actually save me time as a developer. The experiment conducted in the paper simply used subjective information. Every participant was asked how much time they thought SURF would save them, and this information was displayed in a pie chart as a part of their data collection. However, I believed there was a better way to see how much time was saved. The theory behind SURF is that it eliminates sentences it deems to contain no useful information. The way I see it, is that SURF saves you time since you do not have to read those sentences. An unbiased, objective metric to use to assess SURF saves time or not, is to multiply the number of sentences eliminated by the average time it takes to read through one of the review sentences. The study found this time to be 15 seconds, we will call this "t". The number of sentences we will call "n" giving us the equation for "S" (timed Saved):

- S = t x n

Using this equation, here are the results for time saved by app:

| App                      | Time Saved (minutes) |
| ------------------------ | -------------------- |
| Picturex                 | \-5                  |
| PowernAPP                | 123.5                |
| CSTP                     | 2.5                  |
| BLINQ                    | 55.25                |
| Doodle Pairs             | 0.75                 |
| Karaoke SingMe Free/Lite | 8.75                 |
| Karaoke SingMe           | \-6.5                |
| Minesweeper Reloaded     | 2.5                  |
| Sheep-O-block            | 4                    |
| Stone Flood              | 159                  |
| Weight Track             | \-4.25               |
| WifiFileTransfer         | 0                    |
| Video Beta               | \-8.25               |
| Movie Creator Beta       | 36                   |
| TrackID Beta             | 36                   |
| Average                  | 26.95                |

There are multiple takeaways from this data. Namely, that there are four app review summaries that actually produced more sentences than the original data set of reviews (in the XML format). This causes the negative values, meaning Picturex (for example) would ADD five minutes of time if using SURF. Contrast this with the whopping 123.5 minutes saved when using SURF on the reviews for PowernAPP. This is due to the fact that the original XML input file contained over 1,000 reviews and the summary reported about half of that, 556. In my run, it reported even less: the summary reported 173 sentences. This drastic change in sentences saves a lot of time but begs the question: was there some useful information contained in the sentences that were thrown away? Nearly 90% of the review sentences were useless? This seems slightly unrealistic. However, the point stands that the applications with hundreds or even thousands of reviews (PowernAPP, Stone Flood) did save a significant amount of reading for the developer. This seems like the most realistic part to focus on, since a mobile development team for a small application with less than a hundred reviews probably would not find use of a tool like SURF, but bigger companies with popular apps would find the tool most useful. Because of this, I concluded that SURF would be useful in saving developers time in a real world context. 

