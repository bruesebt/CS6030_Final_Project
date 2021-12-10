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
| APPLICATION NAME         | GUI   | APP             | COMPANY | CONTENTS        | DOWNLOAD | FEATURE/FUNC.   | IMPROVEMENT | MODEL           | PRICING | RESOURCES       | SECURITY | UPDATE/VERSION  | TOTAL |
| ------------------------ | ----- | --------------- | ------- | --------------- | -------- | --------------- | ----------- | --------------- | ------- | --------------- | -------- | --------------- | ----- |
| miss-classified          | total | miss-classified | total   | miss-classified | total    | miss-classified | total       | miss-classified | total   | miss-classified | total    | miss-classified | total | miss-classified | total | miss-classified | total | miss-classified | total | miss-classified | total | miss-classified | total | miss-classified | total |
| Picturex                 | 3     | 14              | 2       | 16              | 0        | 0               | 1           | 12              | 0       | 1               | 4        | 21              | 0     | 1 | 4 | 10 | 0 | 4 | 0 | 0 | 0 | 1 | 1 | 2 | 15 | 82 |
| PowernAPP                | 3     | 18              | 3       | 19              | 0        | 4               | 3           | 15              | 1       | 3               | 17       | 65              | 2     | 16 | 2 | 9 | 4 | 11 | 1 | 1 | 1 | 1 | 3 | 11 | 40 | 173 |
| CSTP                     | 1     | 2               | 3       | 10              | 0        | 0               | 0           | 0               | 0       | 0               | 3        | 8               | 1     | 2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 3 | 9 | 25 |
| BLINQ                    | 2     | 6               | 2       | 17              | 1        | 2               | 2           | 12              | 0       | 1               | 4        | 25              | 0     | 1 | 0 | 2 | 0 | 0 | 0 | 0 | 0 | 10 | 1 | 5 | 12 | 81 |
| Doodle Pairs             | 0     | 1               | 0       | 10              | 0        | 0               | 0           | 3               | 0       | 1               | 0        | 8               | 0     | 0 | 0 | 1 | 0 | 1 | 0 | 2 | 0 | 0 | 0 | 1 | 0 | 28 |
| Karaoke SingMe Free/Lite | 1     | 2               | 1       | 18              | 0        | 0               | 0           | 10              | 0       | 4               | 1        | 22              | 0     | 0 | 0 | 0 | 0 | 1 | 0 | 1 | 0 | 0 | 0 | 1 | 3 | 59 |
| Karaoke SingMe           | 1     | 8               | 0       | 11              | 0        | 0               | 0           | 3               | 0       | 0               | 3        | 20              | 0     | 1 | 1 | 4 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 1 | 5 | 49 |
| Minesweeper Reloaded     | 0     | 13              | 1       | 11              | 0        | 0               | 0           | 1               | 0       | 1               | 10       | 23              | 1     | 3 | 0 | 1 | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 5 | 12 | 59 |
| Sheep-O-block            | 0     | 1               | 0       | 7               | 0        | 0               | 0           | 0               | 0       | 1               | 0        | 8               | 0     | 0 | 0 | 1 | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 19 |
| Stone Flood              | 6     | 19              | 6       | 27              | 0        | 0               | 1           | 11              | 0       | 5               | 7        | 58              | 1     | 11 | 1 | 12 | 2 | 10 | 0 | 0 | 0 | 0 | 0 | 15 | 24 | 168 |
| Weight Track             | 1     | 8               | 4       | 13              | 0        | 0               | 0           | 1               | 0       | 0               | 2        | 15              | 0     | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 7 | 38 |
| WifiFileTransfer         | 1     | 1               | 5       | 13              | 0        | 0               | 3           | 5               | 0       | 1               | 5        | 16              | 0     | 0 | 4 | 4 | 0 | 0 | 0 | 1 | 0 | 0 | 1 | 1 | 19 | 42 |
| Video Beta               | 20    | 36              | 7       | 24              | 1        | 2               | 2           | 8               | 1       | 12              | 23       | 84              | 1     | 4 | 2 | 11 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 18 | 57 | 199 |
| Movie Creator Beta       | 10    | 29              | 3       | 16              | 0        | 0               | 4           | 7               | 0       | 0               | 7        | 46              | 1     | 6 | 0 | 3 | 0 | 0 | 0 | 1 | 0 | 0 | 2 | 9 | 27 | 117 |
| TrackID Beta             | 2     | 30              | 1       | 17              | 0        | 0               | 3           | 22              | 0       | 3               | 12       | 56              | 0     | 4 | 0 | 7 | 0 | 1 | 0 | 0 | 0 | 3 | 3 | 18 | 21 | 161 |
| TOTAL                    | 51    | 188             | 38      | 229             | 2        | 8               | 19          | 110             | 2       | 33              | 98       | 475             | 7     | 50 | 14 | 65 | 6 | 30 | 1 | 6 | 1 | 16 | 12 | 90 | 251 | 1300 |
| Correctness rate         | 0.73  | 0.83            | 0.75    | 0.83            | 0.94     | 0.79            | 0.86        | 0.78            | 0.80    | 0.83            | 0.94     | 0.87            | 0.81  |
