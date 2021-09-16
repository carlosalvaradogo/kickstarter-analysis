# Kickstarting with Excel

## Overview of Project

### Purpose

#### The purpose of the analysis was to delve into a Kickstarter dataset to extract insights that would serve to elucidate the following two matters: 1) how campaigns categorized as "theater" fared in terms of outcome according to their launch date, and 2) how campaigns subcategorized as "plays" fared in terms of outcome according to their goals. 

### Background

#### The analysis was carried out against the background of a request by an aspiring playwright, Louise, and her play "Fever", that having come close to achieving her fund-raising goal is now looking for insights into the matters specified under "### Purpose" (see above).

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

#### This particular aspect of the project was concerned with analyzing the outcome of campaigns categorized as "theater" according to their Launch Date. It involved the construction of a pivot table that would count the intances of campaigns categorized as "theater" having achieved a particular outcome (out of three possible: "successful", "failed", and "canceled") and arranging them according to the month of their launch date. Addittionaly, a line graph was produced to facilitate the observation of trends and reach the conclusions that will be discussed below.

### Analysis of Outcomes Based on Goals

#### This particular aspect of the project was concerned with analyzing the outcome of campaigns subcategorized as "plays" according to their goals. It involved the construction of a pivot table that would count the intances of campaigns subcategorized as "plays" having achieved a particular outcome (out of three possible: "successful", "failed", and "canceled") and subsequently calculating the porcentages that the number of instances represented with respect to the total number of campaigns and arranging them according to determinate funding goal ranges. Addittionaly, a line graph was produced to facilitate the observation of trends and reach the conclusions that will be discussed below.

### Challenges and Difficulties Encountered

#### The only challenge or difficulty faced was related to the computing of the number of observations that belonged to each particular range of funding goals in the "Outcomes Based on Goals" part of the analysis. Specifically, utilizing the "COUNTIFS" function, the criteria with which to filter for campaigns subcategorized as "plays" was omitted, such that both the porcentages calculaste and the line graph displayed wrong calculations. The fix involved simply correcting the formula so as to include the missing conditional.

## Results

### Two conclusions to be drawn about the "Outcomes Based on Launch Date" part of the analysis are the following. Firstly, observing the line graph (see above), the "successful" and "failed" lines somewhat mimick each other, such that one can speculate that the proportions of campaigns that are "successful" or "failed" is relatively fixed. This could imply a host of things. One explanation could be that available funding is a function of goals amount for any given month. Secondly, one can observe that, historically, May and June seem to be the two months with the highest number of campaigns with "successful" outcome.

### Two conclusions to be drawn about the "Outcomes based on Goals" part of the analysis are the following. Firstly, and looking at the graph (see above), the lines corresponding to "succesful" and "failed" outcomes visibly mirror eachother. This is, trivially, the result of the fact that our graph is utilizing percentages and there are 0 "canceled" outcomes, such that any increment in "succesful" campaigns as a percentage of total directly implies a reduction of "failed" campaigns as a percentage of total, and vice versa. Also, the number of total campaigns dramatically drops of after the four smallest bins, such that we cannot trust that percentages for all other bins will be stable enough in out-of-sample conditions. Secondly, and somewhat inversely from the last obersvation, the first four bins contain most of the information. For these four bins, "succesful" campaigns are more common than "failed" ones in a decreasing manner as the amount of the goal is augmented.

### One limitation of the dataset, is that it does not contain enought details about the campaigns with which one could evaluate whether the goal for any given campaign is above and beyond what is required. In other words, we cannot evaluate is certain campaigns have inflated goals that may lead us to over-estimate the likelihood of "failed" outcomes.

### One table that we could make to complement the analysis would be one that calculates the average absolute deviation of Pledges around their Goals, organized according to category. The end product would give us an impression of the typical error by category when setting campaign Goals.
