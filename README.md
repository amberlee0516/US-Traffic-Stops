# Data Analysis of US traffic stops

Concern over racial profiling has led to mass collection of traffic stop data. As the data has been made available to the public, researchers have modeled the data to look for evidence of discrimination. This repository includes two projects analyzing 57 datasets of police traffic stops from the [Stanford Open Policing Project](https://openpolicing.stanford.edu/data/). 
* The first project was a general data exploration conducted in Spring 2020 as part of a Data Science Research Circle supervised by [Professor Jo Hardin](https://github.com/hardin47) and [Professor Sarkis](https://github.com/taroub). We used a logistic regression to find that Black motorists are searched at higher rates than white motorists. 
* The second project was completed in Winter 2020 and extensively visualized trends of missing values (missingness) in each  datasets.

## Evidence of non-random missing values in traffic stop data (Winter 2020)

Logistic regression is the most common model applied to traffic stop data, but it is unable to handle missing values. What happens when rows with missing values are naively removed? We know that missing values that are completely random do not introduce bias, but the following visualizations suggest evidence that police agencies change their data reporting behavior based on the time of day. 

I defined a simple metric, the stop missingness rate (SMR) as the percentage of missing values in one row of the data. The SMR can be calculated on the dataset level to assess the amount of missing values. But a more interesting application is to restrict the SMR by a variable, such as race or time, and see how the rate of missingness changes across values of race or time of the day.

A summary of my independent project can be viewed in this presentation (https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/blob/master/2021%20presentation/11_05.pdf). 

##### Missingness across race are similar.

<img src="https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/blob/master/missingness%20final/viz%20for%20eusr%20presentation/fig/SMR_by_race.png" alt="Stop missingness rate by race" width="600"/>

The distribution of SMR for motorist race appears to be about the same. The only difference is that when the motorist race itself is missing, then the SMR is much higher.

##### Missingness across time is different.

<img src="https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/blob/master/missingness%20final/viz%20for%20eusr%20presentation/fig/smr_daynnite.png" width="600" />

<img src="https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/blob/master/missingness%20final/viz%20for%20eusr%20presentation/fig/smr_temporal.png" width="600" />

This plot shows only four datasets, but it summarizes how data reporting practices change across year and time of day. The amount of data available in one year is different from the amount of data in another. Removing observations that are non-randomly missing introduces bias, overweighting instances of traffic stops that police officers report and underweighting the traffic stops that police officers fail to report. 

## General EDA of traffic stop data (Spring 2020)


![race-specific age densities of stopped motorists for different datasets](https://github.com/Amber-Patricia-Lee/US-Traffic-Stops/blob/master/2%20data%20exploration/Nationwide%20visualizations/racial%20age%20distribution%20without%20fill.png)

The final group report is available [here](https://hardin47.github.io/TrafficRC2020/Report/). I  contributed to section 2 (Literature Review) and 3.3 (Nationwide Functions), and I also authored the following sections:
- 1.1 Preface
- 5.1 Demographics of Motorists Stopped, Nationwide
- 5.2.1 Stop outcomes from day to night in Oakland, CA
- 6.5 Empirical Search Probabilities Nationwide
