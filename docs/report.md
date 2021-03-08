# Community Analysis of Next Venues in Seattle, WA 

## Introduction

Cross-promotions are an effective way for businesses to jointly promote their businesses and products or services while reducing marketing costs. These could include giving out coupons for a partner business or doing community events such as "bar hop bingo" to promote a set of local bars and pubs or as part of a fundraising event. However, as a business owner, it may be difficult to strategically decide which other business or businesses would be effective partners to target. Alternatively, as a community event planner it may be difficult to know which venues people would likely travel between in a punch card/bingo-type weekend event. Additionally, an individual business owner may want to know which venues customers typically visit prior to visiting their business, or which places customers travel to afterwards, in order to effectively place advertisements. These types of decisions are often simply based on geographical closeness, using the assumption that people often travel between venues which are near each other. However, locations that are near each other do not necessarily draw from the same customer base, due to a variety of factors such as prices, style, culture and offerings. Likewise, venues which may be located in entirely different neighborhoods may still be connected in terms of how customers go from one to another. Identifying clusters of locales based on where people typically go to and from would allow a more robust analysis of which businesses should partner for joint promotions or advertising. 


## Data 

In order to identify communities of venues which customers typically travel between, we can use the Foursquare venues data. Specifically, the "next venues" endpoint provides information on the top five venues customers typically go to next after a specified venue. We will first "seed" our dataset with a few initial venues via the Foursquare "explore" endpoint, which will return venue recommendations within a specified radius of some geographical coordinates. From that initial list, we can get the venues people typically visit next using the "next venues" endpoint. Once we have that, we can use the "next venues" as the list of venues to query next, and then their "next venues" as the list to query after that, so on and so forth until we reach a sizeable dataset. From this data we will be able to build out a directed network of how venues are connected via their "next venues", with the nodes being the venues and the edges representing the movement of people from one venue to the next. We can weight the edges based on if the next venue was the first, second, third, fourth, or fifth next venue on the list, since the Foursquare data returns next venues sorted by number of people reporting they went there next. From this network of venues we will be able to detect communities of highly-connected venues in order to answer which venues are often travelled between (i.e. those in the same community).  For this particular study we will look at venues in Seattle, WA, with the ten initial venues located within a two-mile radius of downtown, however, this type of analysis would be applicable in any city. 


## Methodology

## Results

## Discussion 

## Conclusion

