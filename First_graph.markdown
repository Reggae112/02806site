---
layout: page
title: Assignment 2 - Investigation of SF crime Data
permalink: /page1/
---

<figure markdown="span">
    ![Header image](/Scary_trend.png)
</figure>

## Rise in forcible sexual offenses in the Bay Area

#### Introduction
Since 2003 San fransisco has been keeping a registry of all reported crimes. This allows us to look into both trends ands specifics of the crime data, the dataset contains data about the crime categories as well as temporal and geographic data, all of which we will use to examine an intersting trend that San Fransisco is experiencing. When looking at the overall dataset, the rise of one particular crime type came to our eye: forcible sexual offenses. At a first glance, this crime type seems to consistently increase in numbers every year, so we decided to look closer and further examine the hypothesis that San Fransisco is indeed experiencing a rise in forcible sex offenses(FSO).
![My image](/SC_trend.png)

#### Understanding the trend
In the above figure, we clearly see how the amount of FSOs are on a steady climb, at a rate much higher than the general development of reported crimes. This begs the question, what is it that is driving this ever increasing amount? Is it because of increasing crime number or due to a larger focus on the crime type from both law enforcement and citizens which leads to increased reporting. Such concepts can be hard to analyze on a quantitative level, one way we can try to get more insight is to examine the development of sex offenses in a more broad spectrum and see if this is an isolated trend or whether its part of a bigger picture. In the figure below you can see a comparison between the different types of sex related offenses and how their relative amount of the total reported crimes has developed over the years. 

#### A look into the geography of sex crimes
{% include Final_map.html %}

The map above shows the geographical distribution of FSOs for each of the years within the dataset. District borders have been highlighted and the number of total forcible sex offenses can be viewed by clicking on the district markers. When we view the map we see the same trend of increasing crimes as in the previous plot. Although it generally appears as if there is an increase in FSOs across all districts, there seem to be two hotspot-areas(marked by red circle) with Tenderloin and its bordering districts and Mission having a much higher concentration of FSOs and what also appears to be a steeper increase in crime numbers across time. When looking into these areas we find that these aren't the poorest, most densely populated or ethnically diverse areas [[5]](https://sfstandard.com/2022/12/08/san-francisco-neighborhood-new-census-data-maps/){:target="_blank"}{:rel="noopener noreferrer"}, instead when we look closer at the specific areas within the districts which are affected by FSOs we see that these are closely related to party culture, take "Valencia street" and "Union Square" which are both part of the highlighted hotspots AND on a list of "The Best Streets for Bar Hopping in San Francisco" by SFtravel.com [[6]](sftravel.com/article/best-streets-bar-hopping-san-francisco){:target="_blank"}{:rel="noopener noreferrer"}. Another interesting trend is that there seem to be a higher number of crimes in areas sorounding train/tram lines, although this might just be due to the increased number of people passing through these areas. 

#### Crime rate of the individual districts
Although the heat map provides a good visual overview of the development of FSOs across time, it can be difficult to accurately tell more how large an increase a given district has experienced and how the different years compares. The plot below therefore shows the development in FSOs of each district along with a trendline summarizing the development in crimes across time. The plot is interactive and each individual district can be turned on and off by clicking on its corresponding legend. When looking at the plot we can first of all see that all trendline slopes are positive conmfirming our impression of an upgoing trend in FSOs. Similarily we also see some areas experiencing a much higher rate of increase in FSOs, with Mission having a more than 10 times higher increase rate than Richmond. 
{% include inter_plot.html %}

#### Conclusion
All in all it is safe to say that San Fransisco is suffering from an increase in FSOs, and that some areas are more affected than others. Districts like Mission and Southern have both a much higher number of FSOs and have also experienced a much higher increase in FSOs across time compared to areas like Bayview and Richmond. It is hard to conclusively come with a reason for this, although it does appear as if areas with more partying have a higher rate of FSOs. For future investigations it could be interesting to further investigate the partying hypothesis and see if FSOs are correlated with large holiday events like new years eve or other temporal patterns. Similarily San fransisco is known for being a university town and looking into wheter any patterns related to student behaviour would be present in the data. This is especially interesting as San Fransisco established a task force aimed at dealing with sexual assault in relation to schools and universities in april of 2016 
[[7]](https://sfgov.org/dosw/sites/default/files/Safer%20Schools%20Sexual%20Assault%20Task%20Force%20Report.pdf){:target="_blank"}{:rel="noopener noreferrer"}
.


#### Reference Links

[SF downtown image](https://cdn.britannica.com/51/178051-050-3B786A55/San-Francisco.jpg){:target="_blank"}{:rel="noopener noreferrer"}

[Article [1]](https://hoodline.com/2024/03/san-francisco-man-convicted-for-sexual-assault-of-elderly-woman-faces-up-to-10-years/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [2]](https://www.cbsnews.com/sanfrancisco/news/san-francisco-man-horrific-child-sexual-assault-facing-50-years-to-life/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [3]](https://sfist.com/2015/11/24/sf_state_officials_refuse_to_commen/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [4]](https://www.eastbaytimes.com/2016/10/23/bay-area-colleges-keep-most-sexual-assault-reports-quiet/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [5]](https://sfstandard.com/2022/12/08/san-francisco-neighborhood-new-census-data-maps/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [6]](https://www.sftravel.com/article/best-streets-bar-hopping-san-francisco){:target="_blank"}{:rel="noopener noreferrer"}

[Article [7]](https://sfgov.org/dosw/sites/default/files/Safer%20Schools%20Sexual%20Assault%20Task%20Force%20Report.pdf){:target="_blank"}{:rel="noopener noreferrer"}

