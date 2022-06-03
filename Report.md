# Abstract
With the expansion of human habits at the expensive of natural and native habits, animal species have to adapt to their new found environment. Most of these changes come in the form of behavioral changes. The Central Park Squirrel Census is a collection of 3,023 squirrel sightings with 31 different data points recorded for each sighting. Of note are behavioral attributes like "Tail Flagging," “Approaches,” “Indifferent,” and “Runs From” in reference to humans. This study uses those four variables to analyze squirrel behaviour with in Central Park. The analysis done is numerical comparison and optical analysis of scatter plots.

# Introduction
## Motivation
As human populations explode, new housing developments consistently encroach on native wildlife habitats. Most often this results in a significant decline in native species and wildlife as the fauna struggle to adapt to the rapid environmental changes, however certain animals such as squirrels find niches in the new urban jungles. Through this final, I hope to explore how this environmental change affects squirrel behavior by analyzing the 2018 Central Park Squirrel Census (https://data.cityofnewyork.us/Environment/2018-Central-Park-Squirrel-Census-Squirrel-Data/vfnx-vebw) to find trends in human-squirrel interaction and how these trends differ from wild squirrels. This data set is a compiled list of squirrel sightings within Central Park by volunteers. The sightings record: details about the fur color of the squirrels, lat & long, and behavior booleans, and is free to use with no restrictions due to its posting on the 'opendataNYC' website.(https://opendata.cityofnewyork.us/faq/)

# Background
## What is known
In 2008 Parker T.S. & Nilon C.H. (http://dx.doi.org/10.1007/s11252-008-0060-0) established that Gray Squirrels show heightened aggression and a decrease in fear response through synurbanization (the process of adapting to an urban environment). Although they use density to proxy synurbanization this is still a foundational study for my analysis. The Parker T.S. & Nilon C.H. paper established a baseline for aggression and fear response which I can use to compare to when modeling the Central Park squirrels.<br>

Eric J. Gustafson and Larry W. VanDruff (https://doi.org/10.2307/2425772) studied the difference between different morphs of grey squirrels. Their findings suggest that different colors of fur do not affect squirrel behaviors. From Eric J. Gustafson and Larry W. VanDruff, I learned that I do not need to control for the morphology of the squirrels in the data set.<br>

Hopewell L. J. et. al. (http://dx.doi.org/10.1111/j.1439-0310.2008.01554.x) studied the hoarding behavior of squirrels in the presence of conspecifics (other squirrels of the same species). They found that in the presence of conspecifics squirrels bury food closer to the source than when food is scarce and conspecifics are not present. From Hopewell et. al. I may be able to theorize if squirrels view humans in the same vein as other squirrels when deciding how far away to bury their food. <br>

# Methodology
## Research Questions
R1 What is the impact of daily human presence on squirrel behavior specifically wariness? 
    
    R1.1 Do squirrels closer to the edge of the park exhibit different behavior than squirrels further from the city?
    
R2 Do squirrels trapped within the environment of NYC exhibit behavior different from squirrels from other cities?

## Methods
Since this data is already gathered I will be mainly preparing the data and analyzing the results. This will be first checking to make sure there are no null values and if so how many and where the null values are. This will give me familiarity with the dataset as well as make sure that the results have been standardized and values are reasonable. Then I will use the recorded lat & long of the squirrels to create a new column for the distance to the edge of the park. This will be my proxy to human presence as I expect squirrels that are closer to the edge of the park to come in contact with humans more, not just walking humans but also the sounds of the city & cars. I need a proxy for this because the dataset does not record the distance from the observer. Finally, I will also compare the clusters of certain behaviors found in this dataset to the average distance for all squirrels and look for notable differences for: 
<ul> <li>Aggresion modeled by tail flagging - "Flagging is a whipping motion used to exaggerate squirrel's size and confuse rivals or predators."
<li> Runs From - Measure of squirrel weariness towards humans
<li> Approaches - Measure of how many squirrels approach humans & are comfortable around humans
<li> Indifferent - Measure of how many squirrels are in the middle of 'runs from' & 'approaches' </ul>

# Discussions
## Findings
After graphing the four behaviors into scatter plots no discernible difference could be found. So the data was put into a numerical format and the average distance to the edge of the park was found. All averages were within .01 units of each other with each unit being which is very roughly around 1 meter if you average the difference between 1 minute of latitude and 1 minute of longitude. To double-check that there was no significant difference I calculated and compared the standard deviations and also found less than a 0.005 unit difference between them which equates to roughly 50 centimeters. This means my results yielded no significant findings and that within Central Park there is not a difference in squirrel behavior and distance to the edge of the park.

## Limitations
My study had several limitations:
The first issue with this analysis is within the dataset. The distance from the squirrel for each behavior sighting is not recorded. This makes it impossible to identify if the squirrel was aware of the human observer and how much influence the human had on the squirrel's behavior. Worse still all other literature regarding squirrel weariness is calculated using distance till flight (DTF) which is how close a human can get before a squirrel runs away. And since all other squirrel data is recorded DTF they use much smaller sample sizes meaning I could not use the ratio between the observed behaviors as a metric either.  
The second major issue with my analysis which in hindsight is much more significant and predictable is that squirrels roam within a 2-mile radius. Central Park is 0.5 miles wide which means no matter where the squirrel's home is within the park they will explore up to at least 2 of its edges. This means that it would make sense that there is not a difference in behavior as all squirrels would have more or less the same urbanized behavior, and without another dataset to compare to this data tells us very little about the squirrels in central park.

# Conclusion
Through lax analysis and a little too little forethought, I have established the squirrel census dataset for Central Park to be very little help for squirrel behavioral research. However, I did establish the behavior of squirrels within Central Park is uniform in regards to distance to the edge of the park. Future analysis of this dataset should instead focus on mapping out human heat maps of the park and comparing the observed behaviors to the park to that, although that runs into a cofounder of the volunteers who recorded this dataset probably used those trails too so naturally, the dataset is biased to record more behaviors next to those trails. My final thought would be for the next squirrel census to record the distance to squirrels to make the data much more usable and comparable to other scientific analyses. 

# Refrences 
Parker, T.S., Nilon, C.H. Gray squirrel density, habitat suitability, and behavior in urban parks. Urban Ecosyst 11, 243–255 (2008). https://doi.org/10.1007/s11252-008-0060-0

Gustafson, Eric J., and Larry W. VanDruff. “Behavior of Black and Gray Morphs of Sciurus Carolinensis in an Urban Environment.” The American Midland Naturalist 123, no. 1 (1990): 186–92. https://doi.org/10.2307/2425772.

Lucy J. Hopewell, Lisa A. Leaver, Stephen E.G. Lea, Effects of competition and food availability on travel time in scatter-hoarding gray squirrels (Sciurus carolinensis), Behavioral Ecology, Volume 19, Issue 6, November-December 2008, Pages 1143–1149, https://doi.org/10.1093/beheco/arn095

