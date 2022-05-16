# Motivation
As human populations explode, new housing developments consistently encroach on native wildlife habitats. Most often this results in a significant decline in native species and wildlife as the fauna struggle to adapt to the rapid environmental changes, however certain animals such as squirrels find niches in the new urban jungles. Through this final I hope to explore how this environmental change affects squirrel behavior by analyzing the 2018 Central Park Squirrel Census to find trends in human-squirrel interaction and how these trends differ from wild squirrels. 

# Research Question
R1 What is the impact of daily human presence on squirrel reactions to said presence? 
    R1.1 What other squirrel behavior changes from daily human presence?
    R1.2 Do squirrels closer to the edge of the park exibit different behavior than squirrels further from the city? 

# Background
## What is known
In 2008 Parker T.S. & Nilon C.H. established that Gray Squirrels show heightened aggression and a decrease in fear response through synurbanization. Although they use density to proxy synurbanization this is still a foundational study for my analysis.
Eric J. Gustafson and Larry W. VanDruff studied the difference between diffrerent morphes of grey squirrels. Their findings suggest that different colors of fur have no effect on squirrel behaviors.
Hopewell L. J. et. al. studied the hoarding behavior of squirrels in the presence of of conspecifics. They found that in the presence of conspecifics squirrels bury food closer to the source than when food is scarce and conspecifics are not present.

## Implications 
This Parker T.S. & Nilon C.H. paper established a baseline for aggession and fear response which I can use to compare to when modelling the Central Park squirrels.
From Eric J. Gustafson and Larry W. VanDruff I learned that I do not need to control for morphology of the squirrels in the data set.
From Hopewell et. al. I may be able to esatblish if squirrels view humans in the same vein as other squirrels when deciding how far away to bury their food.

# Methodology
## Methods
Since this data is already gathered I will be mainly preparing the data and analysising the results. This will be first checking to make sure there are no null values and if so how many and where the null values are. This will give me familiarity of the dataset as well as make sure that the results have been standardized and values are reasonable. Then I will conduct a linear regression using least-squares to find the R squared and p values between the varied behaviors of the squirrels and distance between the edge of the park. This will be my proxy to human presence as I expect squrriels that are closer to the edge of the park to come in contact with humans more. I need a proxy for this because the dataset does not record distance from observer. Finally I will also compare the percent of certain behaviors found in this dataset to the baseline for aggresion and fear found in Parker T.S. & Nilon C.H. found this should show me if the Central Park squirrels are effected more by synurbanization than squirrels in less developed areas.
## Presentations
Most of my presentations will be bar graphs or pie charts showing the percent of squirrels that preformed X behavior when under observation. A bubble chart may be added to show how multiple different behaviors relate. Finally dot maps may also be present if significant findings are revealed in terms of location. 


# Analysis
The Central Park Squirrel Census is a collection of 3,023 squirrel sightings with 31 different data points recorded for each sighting. Of note are behavioral attributes like “Approaches,” “Indifferent,” and “Runs From” in reference to humans. I plan on using this data to map how squirrels in Central Park, a forest in the center of one of the biggest cities in America, have had their behavior changed by constant exposure to humans and their pets. Unfortunately I could not find the license for this data set, as the City of New York website links it to ‘thesquirrelcensus.com’ which then never mentions a license. I would ask you two (the TA, and Professor) for advice on how to proceed. One big issue with the anaylsis using this dataset is that distance from the squirrel is not recorded, making it hard to identify if the squirrel was aware of the human observer and how much influence that the human had on the squirrel's behavior. 

(https://data.cityofnewyork.us/Environment/2018-Central-Park-Squirrel-Census-Squirrel-Data/vfnx-vebw)

# Peer Feedback
After discussion with my peers I received two major pieces of feedback, the first is that I would need a baseline to compare the squirrel behavior to, and they know of no other squirrel datasets that might be compared to. Second, since any squirrel dataset has to be gathered by humans all data that I would be working with will be biased because of its squirrel behavior in the presence of humans. For the first concern I have found several small n <30 published articles of citizen scientists recording squirrel behavior that I can use if need be. The second is a much more valid criticism that will have to be noted, as squirrel behavior might not have changed at all when no humans are present, but since this research has its foundation in human habitat expansion I find the bias acceptable. Final note here, is that my peers were expressly interested in how the squirrels diet may have changed within urbanized environments but that is outside of the scope of this dataset.

# Unknowns and Dependencies
The biggest dependency of this project is setting up a squirrel behavior ‘baseline.’ If no other database or literature can be found on this subject this project can be the first step in establishing that baseline, at least for squirrels in central park. 

# Refrences 
Parker, T.S., Nilon, C.H. Gray squirrel density, habitat suitability, and behavior in urban parks. Urban Ecosyst 11, 243–255 (2008). https://doi.org/10.1007/s11252-008-0060-0

Gustafson, Eric J., and Larry W. VanDruff. “Behavior of Black and Gray Morphs of Sciurus Carolinensis in an Urban Environment.” The American Midland Naturalist 123, no. 1 (1990): 186–92. https://doi.org/10.2307/2425772.

Lucy J. Hopewell, Lisa A. Leaver, Stephen E.G. Lea, Effects of competition and food availability on travel time in scatter-hoarding gray squirrels (Sciurus carolinensis), Behavioral Ecology, Volume 19, Issue 6, November-December 2008, Pages 1143–1149, https://doi.org/10.1093/beheco/arn095