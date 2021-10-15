# US traffic stops

Data analysis of US traffic stops, using R. Updated in winter 2020, this repo also contains my independent research of missingness in traffic stop data that I conducted with Professor Jo Hardin in the fall semester. The missingness project is in [missingness final](https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/tree/master/missingness%20final). One visualization from this project demonstrates how missingness (which I quantify by the stop missingness rate, the SMR) varies. These three datasets from the South are not representative of all datasets but capture the main non-random trends.

![South weekly stop missingness over time](https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/blob/master/missingness%20final/viz%20from%20final%20paper/South%20weekly%20SMR.png)

The final group report from our spring 2020 data exploration is available here: [https://hardin47.github.io/TrafficRC2020/Report/](https://hardin47.github.io/TrafficRC2020/Report/). Sections 5.1, 5.2.1, 6.5, and 1.1 were written by me; I also contributed to sections 2 and 3.3.

This repository contains code for reproducing the visualizations from those sections and more.

Here is one such visualization that shows the race-specific age densities of stopped motorists for different datasets. More visualizations can be found in the final report or within the [data exploration folder](https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/tree/master/2%20data%20exploration).

![race-specific age densities of stopped motorists for different datasets](https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/blob/master/2%20data%20exploration/Nationwide%20visualizations/racial%20age%20distribution%20without%20fill.png)

## Organization of repo

- **1 literature (general)** contains a collection of articles that I referred to throughout the semester
- **2 data exploration** contains all of my data analysis, organized in several folders. Each folder contains data visualizations and the RMarkdown files* that were used to create them.
- **3 logistic regression (paper writing)** contains the progress I have made so far towards turning our data analysis into a paper. 
- **4 scratch** contains a miscellaneous collection of code and external resources
- **5 literature fall 2020** contains data quality and prediction model literature that I read for my independent research project in fall 2020
- **missingness final** is the final product of my independent research project in fall 2020. It contains the framework for stop missingness rate (SMR), exploration of SMR by time and day, and the final paper summarizing my results.

\*Our research circle relied on a private SQL database to store the traffic stop datasets, so I editted each RMarkdown file to remove the passcode for our private SQL connection.

## About the project

This repository contains my personal contributions to a research project analyzing traffic stop data from the [Stanford Open Policing Project](https://openpolicing.stanford.edu/data/). This research began in spring 2020 through a half-credit course, Data Science Research Circle, offered by Pomona College's math department and supervised by [Professor Jo Hardin](https://github.com/hardin47) and [Professor Sarkis](https://github.com/taroub). Currently, we are currently in the process of refining our logistic regression model to write a paper for summer 2020. More about the research circle can be found through Professor Hardin's repository [here](https://github.com/hardin47/TrafficRC2020).

The final group report is available [here](https://hardin47.github.io/TrafficRC2020/Report/). I  contributed to section 2 (Literature Review) and 3.3 (Nationwide Functions), and I also authored the following sections:
- 5.1 Demographics of Motorists Stopped, Nationwide
- 5.2.1 Stop outcomes from day to night in Oakland, CA
- 6.5 Empirical Search Probabilities Nationwide
- 1.1 Preface
