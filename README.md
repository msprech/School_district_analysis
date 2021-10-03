# School_district_analysis

Overview of the school district analysis: Explain the purpose of this analysis.

Initial analysis provided a snapshot of key metrics for the school district in order to show performance patterns and provide additional insight into how student funding impacts student testing scores. However, there was evidence that the original csv had been altered, in particular, the reading and math scores for ninth graders at Thomas High School were suspected of being inaccurate. 

This report seeks to reduce the impact of the false scores on the analysis by first replacing the Thomas High School ninth grade scores with NaN values, and then recalculating the analysis while excluding the ninth grade scores entirely. 


Results: 

* How is the district summary affected? 

The new district summary showed that the percent passing in math, reading, and overall each dropped, however none were a significant change and stayed within a margin of 1%. 

![new district](https://github.com/msprech/School_district_analysis/blob/460d368980014276dd308effb753b7f79f80a62d/Resources/new%20district%20summary%20df.png)

![original district](https://github.com/msprech/School_district_analysis/blob/460d368980014276dd308effb753b7f79f80a62d/Resources/old%20district%20summary.png)


* How is the school summary affected?

By replacing the 9th grade reading and math scores from the students of Thomas High School with NaN (not a number) values, the percent passing both in each subject and overall plummetted. 

![school summary nan](https://github.com/msprech/School_district_analysis/blob/460d368980014276dd308effb753b7f79f80a62d/Resources/THS%20school%20summary%20w%20nan.png)

By recalculating the school summary while excluding these scores completely, only the average math scores and percent passing math suffered. The reading scores, percentage, and overall passing percentage actually improved by dropping the 9th grade scores.  

![school summary no nan](https://github.com/msprech/School_district_analysis/blob/460d368980014276dd308effb753b7f79f80a62d/Resources/THS%20school%20summary%20without%209th%20graders.png)

* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Thomas High School was originally the second highest performing school in terms of overall passing percentage. In replacing the ninth grade math and reading scores with NaN values, Thomas High School dropped out of the top 5, but did not impact the original bottom 5. 

![new top 5](https://github.com/msprech/School_district_analysis/blob/460d368980014276dd308effb753b7f79f80a62d/Resources/top%205%20schools%20with%20nan%20values.png)

How does replacing the ninth-grade scores affect the following:
* Math and reading scores by grade: The average math score dropped from 78.99 to 78.93
* Scores by school spending
* Scores by school size
* Scores by school type


Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
