---
layout: page
title: Life in Bustling Cities
subtitle: How do people move in New York and Tokyo?
cover-img: /assets/img/ny.jpg
thumbnail-img: /assets/img/ny.jpg
share-img: /assets/img/ny.jpg
tags: [books, test]
use-site-title: true
---

Human movement and mobility patterns have been studied on a global scale in the paper “Friendship and Mobility: User Movement in Location-Based Social Network.”  With the use of cell-phone location data as well as two online-based social networks (Gowalla and Brightkite), the authors revealed that human movement can be best summarized as a combination of local repetitive movements and random jumps that highly correlate with their social networks.
Here we’ll be diving into the complex phenomenon of human movement, but in a much more specific context: that of megalopolises!  Indeed, this extension studies the effect of human mobility in much more densely populated areas, New York City and Tokyo.

### The Data Used:
The data we acquired comes from the social media platform “Foursquare”.  This location-based social network provides us with the location and time of anonymous users living in New York City and Tokyo respectively.

_(add logo of FourSquare platform)!_

### Goal: 

Many people move to attractive cities like New York City or Tokyo, looking for an out of habit experience.  But what is actually attractive about such big cities?  The clichés insist that such cities are always buzzing with life, a never ending diversity of activities, daily adventures 	and meeting new people every day.  Let’s find out if this is true!

Here are some interesting questions which we’ll dive into:
Where do city-lovers live?  Are they all clustered in the same place?
How far do people travel from their home?  Are they really discovering new places and being adventurous as they claim to be?
What are these user’s routines? Do New Yorkers and Tokyoites cluster in specific parts of the city during the day?  When are these cities constantly alive and buzzing as they stereotypically seem to be?
What activities are done in such megalopolises? How much diversity is there in the activities done?

## Where do city-lovers live? And are they all clustered in the same place?

After associating home coordinates to each user, according to where they spend most of their time, let’s take a look at where these users live!  Can we identify residential areas?

_(heatmap of user’s homes in both Tokyo and New York city)!_

At first glance, it seems like there are no specific residential areas: the home distribution is quite uniform over both cities.  Indeed, given the high density of population, it would be quite hard to condense users in a single area!

## How far do people travel from their home?  Are they really discovering new places and being adventurous as they claim to be?

Now that we have estimated where every user lives, let’s see how far from their home they like to explore! Do they wander far off and discover new areas or do they restrict themselves to only their neighborhood?

_(Figure showing the probability distribution according the distance from home in km)!_
![distance_from_home](assets/img/distance_from_home.png)
{% include plots/distance_to_home.html %}


Surprisingly, individuals don’t travel that far! According to the plot above, users tend to stay within less than 15 km from their home and rarely wander off.  How far does 15 km look like on a Tokyo and NYC map?

_(Add Tokyo map and NYC map with both a 15 km radius circle superimposed to show how far that distance can look like)!_

<img src="assets/plots/nyc_heatmap.png" width="400">
<img src="assets/plots/tky_heatmap.png" width="400">

If people don’t travel far, what are their habits in this more local environment?

## What are the routines and habits of individuals living in megalopolises?


Now let’s focus more on their daily routines: how do people move during the day and where are they located in NYC and Tokyo respectively?

Below are two interactive maps showing where people are distributed over these megalopolises during the day:

_(add interactive maps with hour by hour evolution of all check-ins)!_
<iframe src="assets/plots/NYC_hourly3.html" width="100%" height="600px"></iframe>    


In these two maps, we can clearly notice that there is an increase in density during the day.  (add more conclusions: people in tokyo are flowing in much later than in nyc, then they leave around XXX hour)

As a result, the center of the respective cities seem to light up during the day, as more and more people are flowing in.  And at the end of the day, some areas are still active, whereas others seem to quiet down.

Another way to look at the user’s movement patterns, is to focus on how many times people report their activity on the Foursquare database during a 24 hour period.  In the histogram below, we quantify the activity of users based on the time of day in both cities.:

_(histogram showing check in hours)!_

Globally, both cities show similar trends; a reduced activity during the night which picks up around 7 a.m. all the way to 11 p.m.  However, we do note some differences between these two cities.  On the one hand, Tokyo reveals a higher activity level from 5 p.m. to 11 p.m. but seems to die down.  On the other hand, New York City shows less activity in the late afternoon, but appears to be more active during the night time.

According to this graph, we could always consider these cities as “cities that never sleep”, but the night activities still remain notably lower compared to the day!

## Now that we’ve seen when the cities are the most buzzing with activities, what type of activities do New Yorkers and Tokyoites actually like to do respectively?

What type of activities are most popular in these dense cities?  We ranked the different types of venues for both New York and Tokyo and here’s what appeared to be most popular:

_(New York histogram)!_

This New York City histogram reveals that one of the most common activities done in this city corresponds to going to bars, followed closely by spending time at home.  As a result, this histogram does reflect this image of a buzzing city with a lot of social encounters.  The following most important activities are going to the office, taking the subway, going to the gym and the coffee shop!

When comparing with popular activities in Tokyo, a surprising activity dominates this city: most of the people spend their time at the train station!  

_(Tokyo histogram with the train station)!_

This dominating activity is followed by people taking the subway and then the following activities are considerably less popular in comparison to being at the train station!
To still get an idea of the scale of the activities other than being at the train station, we removed the first two top activities and looked at the following most popular ones:

_(Tokyo histogram with the train station)!_

The popular activities in Tokyo differ surprisingly from those in New York City: Tokyoites tend to prefer Convenience stores and restaurants.  However, the bar is still among the top 5 activities, but being at home does not appear to be one of the top activities.  As a result, this histogram illustrates that Japan seems to be a city, which indulges more in outside activities rather than staying at home as seen in New York City!


To push this comparison even further, we can compare when the top types of activities are done during the day.  For New York City, we gathered the top venues from the histogram above and saw when these activities were most done for both New York City and Tokyo.  Interestingly enough, despite one city having much more activity in that domain, the peaks are located in both cases at similar hours.  For instance when looking at the category “bar”: one can see that for New York City there is a large peak from 5 p.m. to 5 a.m., but there is a similar and more narrow peak around 5 p.m. to 11 p.m. (maybe make more conclusions)

_(comparing NYC’s top venues in both cities)!_
_(comparing Tokyo’s top venues in both cities)!_

Another interesting way to look at these types of activities, is if we group them into more general categories: “Food”, “Arts & Entertainment”, “Fitness”, “Shopping”, “Work & School”, “Travel & Transport”, “Home & Residential”, and “Nightlife”.

_(Comparing Categorical Venue Types in both cities)!_

What transpires through these plots is that in both cities the trends look very similar. For instance, when looking at either “Food” or “Art & Entertainment”, the same two peaks appear during the same time span.  As a result, we can infer that no matter the city, there are some general periodic patterns that can be clearly identified!

It’s also interesting to note that in the early afternoon, a lot of Tokyoites go home for lunch (as seen with the peak in the “home and residential” around 12 pm to 2 pm), which is pretty different compared to the Tokyoites who prefer to eat out!


One final way to really identify the differences between New York City and Tokyo citizens is by looking at the top venues according to a 6h time period.

_(Add Distributions of top venues according to time periods for both NYC and Tokyo next to each other)!_
![nyc_wordcloud](assets/img/nyc_wordcloud_all.png)
![tky_wordcloud](assets/img/tky_wordcloud_all.png)

This figure really highlights the astounding amount of time Tokyoites spend at the train station during the entire day! Whereas the activities tend to switch during the hours for New York City, the main activity remains constant for Tokyo.


Time of day | **New York** | **Tokyo**
--- | --- | ---
*__06-12__* | Office, Coffee, Gym | Train station 🚉, Subway, Convenience store
*__12-18__* | Home, Office, Food, Gym | Train station 🚉, Subway, Restaurants
*__18-00__* | Bar 🕔😄🍻, Home, Gym 🏋️‍♀️| Train station 🚉, Subway, Bars, Restaurants
*__00-06__* | Bar, Home | Train station, Bars, Convenience Store

<div class="row justify-content-center no-gutters mb-5 mb-lg-0">
      <table class="table table-borderless col-lg-8">
        <thead>
        <tr>
          <th scope="col"  class="bg-dark-red text-white text-center">Time of the day</th>
          <th scope="col"  class="bg-light-sand text-center">New York City</th>
          <th scope="col"  class="bg-light-sand text-center">Tokyo</th>
        </tr>
        </thead>
        <tbody>
        <tr>
          <td class="text-dark-red text-center"><h3><b>06-12</h3></td>
          <td class="text-dark-red text-center"><h1><b>Office</h1>
                                                <h2><b>Coffee</h2>
                                                <h3><b>Gym</h3></td>
          <td class="text-center"><h1><b>Train station</h1>
                                <h2><b>Subway</h2>
                                <h3><b>Convenience store</h3></td>
        </tr>
        <tr>
          <td class="text-dark-red text-center"><h3><b>12-18</h3></td>
          <td class="text-dark-red text-center"><h1><b>Home</h1>
                                                <h2><b>Office</h2>
                                                <h3><b>Food</h3></td>
          <td class="text-center"><h1><b>Train station</h1>
                                <h2><b>Subway</h2>
                                <h3><b>Restaurants</h3></td>
        </tr>
        <tr>
          <td class="text-dark-red text-center"><h3><b>18-00</h3></td>
          <td class="text-dark-red text-center"><h1><b>Bar</h1>
                                                <h2><b>Home</h2>
                                                <h3><b>Gym</h3></td>
          <td class="text-center"><h1><b>Train station</h1>
                                <h2><b>Subway</h2>
                                <h3><b>Bars</h3></td>
        </tr>
        <tr>
          <td class="text-dark-red text-center"><h3><b>00-06</h3></td>
          <td class="text-dark-red text-center"><h1><b>Bar</h1>
                                                <h2><b>Home</h2>
                                                <h3><b>Subway</h3></td>
          <td class="text-center"><h1><b>Train station</h1>
                                <h2><b>Bars</h2>
                                <h3><b>Convenience store</h3></td>
        </tr>
        </tbody>
      </table>
</div>
    
## Conclusion and Implication:

To conclude, big cities share common traits which understandably represent appealing reasons to move. Seeing how densely populated Tokyo and New York City are, there is no doubt that meeting new individuals is effortless.  Moreover, there is a considerable diversity of things to do!  Will you travel and explore farther away from your home than if you lived in some rural city in the Midwest? Probably not, but there is plenty to do right next to you!

_Venn diagram to compare both cities: !_



Such a study and observations can have quite useful implications.  Knowing the user’s locations can definitely contribute to improving urban planning and migration patterns: where would it be useful to construct a new subway line? Would opening a restaurant in Brooklyn work better than opening it in the Bronx?  Such knowledge could also contribute greatly in advertising: when a gym is looking for new memberships, this will enable it to advertise in locations where a lot of people go work out or try to capitalize on a location that doesn’t have many competitors.

Last but not least, understanding this human mobility is valuable information, especially considering the current Covid context.  Seeing human movement patterns can help identify regions where the risks are higher and where clusters tend to be most created.


