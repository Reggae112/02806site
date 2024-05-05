---
layout: page
title: Final Assignment
permalink: /page2/
---

#### Biking and the Big Apple
New York has expressed governmental aspirations to transition into a city with a stronger focus on cycling infrastructure. However, gauging the success of this transition varies depending on the perspective. By analyzing city-collected data, we hope to shed light on the development of bicycle usage and infrastructure throughout this transition, uncovering both progress and areas needing improvement. We will go over both temporal and geospatial dimensions in this development to showcase all there is to know about the two-wheeled revolution. 

#### An Open Data Investigation
- Geojson files of New York district boundaries
- New York City Population By Community Districts
- Bicycle Parking Shelters 
- NYPD Complaint Data Current (Year To Date)
- Bicycle Counts

#### Crime rate of the individual districts
If we take a look at the data collected from counting stations across the city, we see that the city has experienced a drastic increase in bicycle commuters. Especially the years between 2013 and 2016 saw a rapid rise of numbers of cyclists. 

![My image](/AADTINY.png)

There is however an interesting development of 3 consecutive years of negative development from 2016-2019. If we compare this to the intuitive notion that numbers like this would more likely be on a steady climb, it begs the question if there might be something that we are missing. 
If we look at survey data, for example the one presented in
[Survey Data](https://www.nyc.gov/html/dot/html/bicyclists/cyclinginthecity.shtml){:target="_blank"}{:rel="noopener noreferrer"} we see that this development is not present. This source is based on the United States Decennial Census’ American Community Survey. In the data displayed we see a steady growth, which could lead us to the idea that this trend might have more to do with the way the counting data was created than with the actual development of cyclists itself. Since counting stations are moved, infrastructure is changed (and as such the paths people chose) the bicycle counters become misrepresentative as a measure of the bicycle traffic within the city. If we look within the documentation for the report, we also find the description

*"Bike Use Surveys collect information about cycling from samples of the general population. These surveys do not typically provide information about where people are cycling, but they are more geographically encompassing and can more accurately gauge the number of people who are biking, including those who may not ride past typical count locations or use bike share"*

What we therefore might use this data for, which the surveys don't provide, is to get a geospatial understanding of the development. 

{% include Bike_counts.html %}

But as can be seen from the above plot the counting stations are limited both in numbers, and locations, there are many areas which are completely void of counts.The data is therefore not very good for for doing these geospatial investigations that we want to do.

#### Bike parking as a proxy for biking
Luckily one of the other identified data sets provide us with a better opportunity to asses geospatial tendencies. The below map depicts the desitribution of new bike parking across the different districts of NYC. The data shows a timeseries from 2000 till now and allow us to see how the different districts of NYC has shaped their environments to better fit bikers.

{% include Bike_parkings.html %}

Here we see how Brooklyn districts like Williamsburg and Brooklyn heights have established many times more bike parkings than say Riverdale, Bronx. One of the reasons for this could be that it has become increasingly more popular among tourists to go biking in lower Manhatten and around Brooklyn bridge, with an abundance of different companies providing guided tours along the East River [Survey Data](https://www.tripadvisor.com/Attractions-g60763-Activities-c61-t214-New_York_City_New_York.html){:target="_blank"}{:rel="noopener noreferrer"}. 

One thing is clear and that is that the number of bike parking possibilities has increaed over time. If you hover the mouse over a specific district the plot displays the name of the neighbourhood and the exact number of parkings established since 2000. This plot shows us that the investment in infrastructure is steadily rising, but is far from evenly distributed. Especially less affluent areas see little development compared to the high number of residents. 

#### Crime rate of the individual districts

{% include Bike_theft.html %}


#### Crime rate of the individual districts
Although the heat map provides a good visual overview of the development of FSOs across time, it can be difficult to accurately tell how large an increase a given district has experienced and how the different years compare. The plot below therefore shows the development in FSOs of each district along with a trendline summarizing the development in FSO crimes across time. The plot is interactive, and each individual district can be turned on and off by clicking on its corresponding legend. When looking at the plot, we can first of all see that all trendline slopes are positive, confirming our impression of an upward trend in FSOs. Similarly, we also see some areas experiencing a much higher rate of increase in FSOs, with Mission having a more than 10 times higher increase rate than Richmond. dsf
{% include crime_plot.html %}




![My image](/polar_plot.png)

#### Reference Links

[SF downtown image](https://cdn.britannica.com/51/178051-050-3B786A55/San-Francisco.jpg){:target="_blank"}{:rel="noopener noreferrer"}

[Article [1]](https://hoodline.com/2024/03/san-francisco-man-convicted-for-sexual-assault-of-elderly-woman-faces-up-to-10-years/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [2]](https://www.cbsnews.com/sanfrancisco/news/san-francisco-man-horrific-child-sexual-assault-facing-50-years-to-life/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [3]](https://sfist.com/2015/11/24/sf_state_officials_refuse_to_commen/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [4]](https://www.eastbaytimes.com/2016/10/23/bay-area-colleges-keep-most-sexual-assault-reports-quiet/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [5]](https://sfstandard.com/2022/12/08/san-francisco-neighborhood-new-census-data-maps/){:target="_blank"}{:rel="noopener noreferrer"}

[Article [6]](https://www.sftravel.com/article/best-streets-bar-hopping-san-francisco){:target="_blank"}{:rel="noopener noreferrer"}

[Article [7]](https://sfgov.org/dosw/sites/default/files/Safer%20Schools%20Sexual%20Assault%20Task%20Force%20Report.pdf){:target="_blank"}{:rel="noopener noreferrer"}

