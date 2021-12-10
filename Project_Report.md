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
