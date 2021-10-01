# Kickstarting with Excel
Performing analysis on Kickstarter campaigns using Excel.

## Overview of Project

### Purpose

The goal of this project is to advise a client, Louise (a potential theater director), on the best time to launch a Kickstarter campaign for funding her upcoming play, Fever. This exercise was an introduction on Excel's capabilities creating Pivot Tables, Pivot Charts, Conditional Fomatting, and a number of other functions for statistical analysis that produce graphical representations of data.

## Analysis and Challenges

Analysis for this project began by getting to know the dataset provided for Kickstarter campaigns launched from 2009 to 2017. Our client would like to answer these questions:

  * Is there an optimal time of year to start a theatrical Kickstarter campaign?
  * How do the funding goals for a play effect the its success in Kickstarter?

### Analysis of Outcomes Based on Launch Date

The data provided contains the information we need, but not in the format to easily create graphical representations for quick reference. To begin answering the clients questions, I created a "Years" column by extracting it from the "Date Created Conversion" data given in the orignal set (this was initially provided as Unix timestamps). Using the years, a Pivot table and Pivot chart were generated to see the theater campaign outcomes based on their launch dates. The table filters the "theater" Parent category and removes the "live" outcomes to reflect the clients interests. The chart below shows the graphical representation of the data with "successful" in blue, "failed" in orange, and "canceled" in yellow.

![Outcomes Based on Launch Date](https://github.com/jp3tty/Module-1-Challenge/blob/main/Resources/Theater_Outcome_vs_Launch.png)


### Analysis of Outcomes Based on Goals

To provide the client with information on how the outcomes were influenced by their funding goals, I created the chart below by comparing a given "Outcome" percentage against a campaign goal. To keep the chart from appearing too busy, the entire datasets was filtered to consider only plays, due to the clients interests, and the funding goals were reduced to 12 monetary ranges (valued in US dollars). This analysis can be seen in the chart below.

![Outcomes Based on Goal](https://github.com/jp3tty/Module-1-Challenge/blob/main/Resources/Outcomes%20Based%20on%20Goal.png)

Successful in blue, failed are in orange, and canceled in grey.

### Challenges and Difficulties Encountered

One difficulty that stood out occured when working with the Pivot table for "Outcomes Based on Goals." After working through the Module and manipulating the data in a variety of ways, Excel's data cache had issues referencing the proper values for the data I needed to work with. As a result, the chart that did not match what was expected in the challenge. After a fair amount of troubleshooting, a solution was discovered by preforming a "refresh" directly to the Pivot table. 

## Results

* What are two conclusions you can draw about the Outcomes based on Launch Date?

 1. May appears to be the best time of year to launch Kickstarter campaigns for theater productions. Most of these campaigns are launch  during this month with a steady decline to December.
 2. Theater production Kickstarter campaigns are successful overall. Every month on the chart shows there are more successful campaigns than failed, the worst of which is December where successful and failed campaigns are near equivalent.

* What can you conclude about the Outcomes based on Goals?

  The most outcomes are projects with funding goals that are less than $5,000 or between $35,000 and less then $45,000, and the worst outcomes where between $45,000 to $49,999.

* What are some limitations of this dataset?

  There may be limitation due to the size of the dataset. At just over 4000 data points, I assume we are missing a great deal of information for our analysis, especially considering the international reach of this data and eight year timespan.

* What are some other other possible tables and/or graphs that we could create?

  We could make a variety of different charts based on the success, failure, and cancelation of any other subcategories. In addition, we could chart comparisons between the subcategories to determine how well each preform.


