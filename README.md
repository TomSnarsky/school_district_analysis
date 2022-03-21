# School District Analysis

## Overview of the school district analysis

In this analysis, we looked at reading and math test score data for all of the high schools in one district. To understand this data as completely as possible, we looked at it from many different perspectives and levels of analysis, beginning with broad-strokes district and school summaries and eventually drilling down to analysis by grade level and sorting schools in the district by other parameters like per-capita school spending, school size, and school type in order to ascertain all the different patterns we could. In addition, it was discovered after the initial analysis that there was evidence of academic dishonesty in the data (at Thomas High School), so the analysis needed to be revised to adjust to these anomalies.

## Results

An overview of our results follows below, including comparisons between the original data set and the revised data set.

### How is the district summary affected?

The original district summary is below:

<img width="896" alt="image" src="https://user-images.githubusercontent.com/99628051/159196271-386cefe1-5a23-477b-862d-233e3869164f.png">

After the data was adjusted for the academic dishonesty concerns, the district summary looked like the following:

<img width="899" alt="image" src="https://user-images.githubusercontent.com/99628051/159196580-c9036f13-179a-49cd-95b1-c92e59a5f3d8.png">

As evidenced by the numbers in the table, there was a slight increase in the Average Math Score, the % Passing Math, % Passing Reading, and % Overall Passing. Although the differences are not tremendous in the district summary data, they become more apparent in the school summary data which makes visible the school that was dealing with the allegations, Thomas High School.

### How is the school summary affected?

The initial school summary is shown below:

<img width="989" alt="image" src="https://user-images.githubusercontent.com/99628051/159200202-d7cd8a54-4926-4b63-8583-e1705327da5b.png">

After adjustments for the academic dishonesty concerns for Thomas High School, the revised school summary looked like this:

<img width="986" alt="image" src="https://user-images.githubusercontent.com/99628051/159200252-b8a2da81-641d-489e-9d10-6b9879f382b5.png">

Clearly the differences for Thomas High School were dramatic: although the average scores were not hugely affected because the allegedly-fraudulent scores were replaced with "not-a-number" (NaN) values, the passing rate for math, reading, and overall changed by amounts on the order of thirty percentage points. (This artificial inflation of these rates could be explained by the fact that upperclassmen might have an easier time of passing a state math exam, especially if (as is the case in states like Massachusetts) students are fully prepared for the test curricularly by 10th grade but not by 9th.)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

In the initial analysis, Thomas High School's Overall Passing rate of approximately 65% (as pictured below) places it 8th in the district (which is also 8th from the bottom, since there are 15 schools total).

<img width="987" alt="image" src="https://user-images.githubusercontent.com/99628051/159198374-8507d154-e23a-4988-b8f8-cfb0888c62f5.png">

After the revision, the inflation of Thomas High School's passing rates shoots it up to second (!) in the district by overall passing rate:

<img width="981" alt="image" src="https://user-images.githubusercontent.com/99628051/159198014-12022a02-b19d-41d3-afab-b26eb966c2bf.png">

### How does replacing the ninth-grade scores affect the following:

See each section below for sub-analyses.

#### Math and reading scores by grade

Fortunately, we were able to preserve most of the grade-level data because only the ninth-grade scores from Thomas High School needed changing. This means that we can still see grade-level data from each school including grade-level data from the other grade levels at Thomas High School, like in this image:

<img width="291" alt="image" src="https://user-images.githubusercontent.com/99628051/159198605-d0c9b7cc-fe97-413e-8831-9d8f263e6789.png">

#### Scores by school spending

Initially, the score data by school spending looked like this:

<img width="813" alt="image" src="https://user-images.githubusercontent.com/99628051/159198845-3f5a7de2-4ad3-4b02-95c3-cac2f7b2fdc1.png">

Thomas High School being in the $631-645 range meant that the passing rate was accordingly mildly inflated for that range.

#### Scores by school size

Initially, the score data by school size looked like this:

<img width="745" alt="image" src="https://user-images.githubusercontent.com/99628051/159201023-323ad505-e930-4a40-a005-d5c931098f2e.png">

Thomas High School being in the medium size group meant that the passing rate was accordingly mildly inflated for that subgroup.

#### Scores by school type

Initially, the score data by school type looked like this:

<img width="704" alt="image" src="https://user-images.githubusercontent.com/99628051/159201091-b820a8e7-c895-4805-b551-3ef45ef016d0.png">

Thomas High School being a charter school meant that the passing rate was accordingly mildly inflated for that school type.

## Summary

Our analysis was able to give us several key insights even though the integrity of our data was challenged by the academic dishonesty allegations at Thomas High School. Overall, our four key takeaways from the comparative analysis were as follows: 1) The district summary data was only affected on a very small scale, with changes at the level of a few tenths of a percentage point overall; 2) the school-level data for Thomas High School reflected a massive inflation in pass rates (20+ percentage points in math, reading, and overall) when only upperclassman (grades 10-12) data were considered; 3) this inflation led to changes in the $631-$645 per capita spending, medium school size, and charter school subgroups in the respective broken-down analyses; and 4) cross-school comparisons would still be possible at the 10-12 grade level because we have that grade-level data, so if we wanted uninflated comparisons we could look at 10-12 graders across all the schools to get a sense of how they compared without our analysis being compromised by the academic dishonesty allegations.
