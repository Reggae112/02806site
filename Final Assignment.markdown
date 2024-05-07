---
layout: page
title: Final Assignment
permalink: /page2/
---
![My image](/datavizfrontpage.png)

#### Biking and the Big Apple
New York has expressed governmental aspirations to transition into a city with a stronger focus on cycling infrastructure. However, gauging the success of this transition varies depending on the perspective. By analyzing city-collected data, we hope to shed light on the development of bicycle usage and infrastructure throughout this transition, uncovering both progress and areas needing improvement. We will go over both temporal and geospatial dimensions in this development to showcase all there is to know about the two-wheeled revolution. 

#### An Open Data Investigation
For this investigation the large amount of available data sets provided by the City of New York through their portal NYC Open Data, was utilized. The following data sets layed the ground for this article:
- Geojson files of New York district boundaries
- New York City Population By Community Districts
- Bicycle Parking Shelters 
- NYPD Complaint Data Current (Year To Date)
- Requests for in-building parking
- Bicycle Counts at counting stations

#### Crime rate of the individual districts
If we begin by taking a look at the data collected from counting stations across the city, we see that the city has experienced a drastic increase in bicycle commuters. Especially the years between 2013 and 2016 saw a rapid rise of numbers of cyclists. 

![My image](/counting_station_data.png)

There is however an interesting development of 3 consecutive years of negative development from 2016-2019. If we compare this to the intuitive notion that numbers like this would more likely be on a steady climb, it begs the question if there might be something that we are missing. 

If we look at survey data, for example the one presented in
[Survey Data [1]](https://www.nyc.gov/html/dot/html/bicyclists/cyclinginthecity.shtml){:target="_blank"}{:rel="noopener noreferrer"} we see that this development is not present. This source is based on the United States Decennial Census’ American Community Survey. In the data from the article displayed below, we see a steady growth, which could lead us to the idea that this trend might have more to do with the way the counting data was created than with the actual development of cyclists itself.
![My image](/bicyling_city.PNG)

 Since counting stations are moved, infrastructure is changed (and as such the paths people chose) the bicycle counters become misrepresentative as a measure of the bicycle traffic within the city. If we look within the documentation for the report, we also find the description

*"Bike Use Surveys collect information about cycling from samples of the general population. These surveys do not typically provide information about where people are cycling, but they are more geographically encompassing and can more accurately gauge the number of people who are biking, including those who may not ride past typical count locations or use bike share"*

When we try an look at the temporal trends in the data we also see something suprising. Here it appears as if people are riding their bikes more in the winter. Something which with our newly required knowledge of the uncertainty of bike counting data and our common sense seems somewhat suspect.
![My image](/polar_plot.png)

Another area we might use this data for, which the surveys don't provide, is to get a geospatial understanding of the development. 

{%include Bikecounts.html%}

But as can be seen from confirmed from the above plot the counting stations are limited both in numbers, and locations, there are many areas which are completely void of counts. The data is therefore not very good for for doing these geospatial investigations that we want to do, and we must look elsewhere.

#### Bike parking as a proxy for biking
Luckily one of the other identified data sets provide us with a better opportunity to asses geospatial tendencies. The map linked below(not displayed due to limitaions in the size of files allowed to be pushed to GIT) depicts the desitribution of new bike parking across the different districts of NYC. The data shows a timeseries from 2000 till now and allow us to see how the different districts of NYC has shaped their environments to better fit bikers.

[Bike Parking map](/02806site/parking_map/){:target="_blank"}{:rel="noopener noreferrer"}

Here we see how Brooklyn districts like Williamsburg and Brooklyn heights have established many times more bike parkings than say Riverdale, Bronx. One of the reasons for this could be that it has become increasingly more popular among tourists to go biking in lower Manhatten and around Brooklyn bridge, with an abundance of different companies providing guided tours along the East River [Survey Data[2]](https://www.tripadvisor.com/Attractions-g60763-Activities-c61-t214-New_York_City_New_York.html){:target="_blank"}{:rel="noopener noreferrer"}. 

One thing is clear and that is that the number of bike parking possibilities has increaed over time. If you hover the mouse over a specific district the plot displays the name of the neighbourhood and the exact number of parkings established since 2000. This plot shows us that the investment in infrastructure is steadily rising, but is far from evenly distributed. Especially less affluent areas see little development compared to the high number of residents. 

#### Bike parkings per person 
The previous plots didn't take into consideration the difference of populations of each of the districts. One could imagine that districts with more people probably would have more bike parkings, simply due to the higher population. The map below therefore displays the data normalized in terms of the population of the individual district by looking at the parking per person. Interestingly this plot only seems to exagerate the trend visible on the previous plots with lower manhatten and west brooklyn having a much higher ratio of bike parkings per person. Again similar reasoning can be applied for why, but it is difficult to say exactly

{%include Bikeper_person.html%}

Interestingly if we try and look at how the ratios translate into bikes per person as displayed on the plot below and compares the to same number for cars based on an article named [The Power Of Bicycle Parking[3]](https://transalt.org/reports-list/the-power-of-bicycle-parking){:target="_blank"}{:rel="noopener noreferrer"}, we see how little biking has been prioritized. According to the article there is 1.5 parking spots per car - That is more than one spot per single car! When it comes to bikes the article tells a different story of there being 116 bikes per bike parking spot. Something which if we take into consideration that not everyone has a bike these numbers fit well with our own calculations of an average of 240 people per bike parking. 

![My image](/ratiobars.png)

#### Bike crimes and the NYC
Another interesting dimension is the geographical distribution of bicycle related crimes. Like for the amount of parking the number of bike theft is not nearly the same across town. We have analysed the number of reported bike crimes and how these are distributed in relation to the previous investigated districts. In the below plot, you can take a look at the different types of bicycle crime to see how they distribute themselves throughout the city. Try toggling the different types and see if you find anything interesting. Use the map to help in understanding how it distributes throughout the city. You might notice that some areas are overepresented. This begs the question whether these areas are just more crime stricken or that it might be because of lacking possibilities to find safe parking. Alternatively more streetside parking might also mean that bike theft is actually easiser as people are more prone to park their bikes on the streets where they can be potentially stolen. Or again there might just be that mamy more bikes in areas with proper bike parkings and therefore also many more stolen bikes.

{%include crimeplot.html%}

When we look at how the bike crimes distribute themselves geographically across the city seen on the map below, which shows the total number of crimes combined. We see that it does look slightly familiar to the ones displaying the ratio of bike parking per person. Again whether this is due to more bikes in general or more bikes available for thieving due to outside parking is difficult to say.

{%include Biketheft.html%}

#### Are the NYC bikers satisfied?
So now we have delved into how the number of bike parkings have increased through recent years - but is it enough to satisfy the demand of New Yorkers? One way to investigate this is diving into the logs of requests made to the city for in-building bicycle parking. 

![My image](/parking_request.png)

What we see in the above plot, apart from the interesting seasonal pattern of requests peaking in the summer, is that the requests are approaching 0. This could indicate that the infrastructure investments have suceeded in filling the needs of many cititzens and as such the need for more in-building parking is decreasing. As such, the infrastructure investments seem to be effective. There are of course many unknown variables within this that we have not been able to cover, such as changes in the request process, whether the amount of eligible buildings has been used up etc.

If we look back at other types of data, for example the survey data reviewed when looking at the ratios of bikes and cars to parking, it tells a different story. In the article, [[3]](https://transalt.org/reports-list/the-power-of-bicycle-parking){:target="_blank"}, Transportation Alternatives describes several interesting aspects 

* Currently, there are over 100 times more car parking spaces than bicycle parking spaces, despite more residents owning bicycles than cars.
* This lack of parking discourages people from cycling, with it being the second most common reason people don't bike more.
* The deficit is especially impactful on low-income communities and communities of color, who are more likely to rely on bicycles for transportation and less likely to have access to secure storage.

And as One founder and CEO Shabazz Stuart says in an interview for the article [State Bike Survey Shows Demand for Secure Parking at Transit Hubs by Dave Clon for Streets Blog NYC[4]](https://nyc.streetsblog.org/2022/05/05/state-bike-survey-shows-demand-for-secure-parking-at-transit-stations){:target="_blank"}

*"It's not surprising, I don't know how much more data we need to reach the long overdue conclusion that secure and protected bike parking is essential to a viable cycling-as-transit ecosystem."*

Another aspect is, that for an increase in bike parkings to make a difference it needs to be affordable. Something which is especially the case when considering how low-income areas are the ones the most in need of more space. [An article by the New York Times[5]](https://archive.nytimes.com/cityroom.blogs.nytimes.com/2010/02/23/you-can-park-your-bike-but-at-what-price/){:target="_blank"} reported that the bike parkings required by law in commercial car garages for every 10 cars came at a price *"nearly twice the cost of a monthly metro pass"*. Although the article is relatively old(2010) it still highlights a crucial aspect and bias in who can benefit from inititatives like policy changes if the bigger picture isn't taken into consideration.

#### Final remarks
It seems the transition to a bicycle-dominated infrastructure landscape is still an ongoing story with great variation within the districts of the Big Apple. When trying to explain why some areas are behind and others ahead, it appears as if social inequality and tourism has role to play. There is still much to be wished for from the citizens of New York, but lukily it seems as if we are moving in the rigth direction - More bicycles and more parking for them. The transition might seem inevitable as the city races to meet citizen demand, but as with all other development and investment, it is important that we are mindful of not leaving anyone behind. Luckily datasets such as the ones presented within this article can help us in getting an - if not better then at least differently biased - perspective, that allows us to tell another side of the story of cycling in New York. 

#### Reference Links

[Article [1]](https://www.nyc.gov/html/dot/html/bicyclists/cyclinginthecity.shtml){:target="_blank"}{:rel="noopener noreferrer"}

[Article [2]](https://www.tripadvisor.com/Attractions-g60763-Activities-c61-t214-New_York_City_New_York.html){:target="_blank"}{:rel="noopener noreferrer"}

[Article [3]](https://transalt.org/reports-list/the-power-of-bicycle-parking){:target="_blank"}{:rel="noopener noreferrer"}

[Article [4]](https://nyc.streetsblog.org/2022/05/05/state-bike-survey-shows-demand-for-secure-parking-at-transit-stations){:target="_blank"}

[Article [5]](https://archive.nytimes.com/cityroom.blogs.nytimes.com/2010/02/23/you-can-park-your-bike-but-at-what-price/){:target="_blank"}