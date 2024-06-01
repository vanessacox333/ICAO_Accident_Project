# ICAO_Accident_Project

This analysis was motivated by the early 2024 Boeing media craze. The media seemed out to get Boeing, with news stories all around the world covering Boeing accidents/incidents for weeks on end. Is Boeing actually significantly more dangerous than other airplane manufacturers? Or is this another media conspiracy, driven by the desire to get views, likes, and clicks? The goal of this analysis was to gain some insight into which plane manufacturer has the most accidents, how accident occurrence has changed over time, what is the most common cause of airplane accidents, etc. The data set was gathered using the ICAO API Data Service and consists of all accidents around the world reported by the ICAO from 2008-2022.

I would like to add in a couple caveats prior to discussing our results. The first being that the reference database we used to retrieve manufacturer names did not use consistent naming conventions. We accounted for this by manually creating a mapping dictionary where we researched and grouped the manufacturers to the best of our abilities. We are not experts in the aviation industry; there have been countless mergers, crossovers, collaborations, etc. between manufacturers which caused some confusion with grouping. For example, Cessna and Beechcraft are owned by Textron so listing the 'correct' manufacturer is based on a variety of factors we were unable to account for. Collaboration with experts in the field could resolve some of these issues and change results in the future.

The second caveat is we are dealing with count data, not proportion data. It should intuitively make sense that the largest plane manufacturers would have more accidents than smaller plane manufacturers based on the fact that they have more planes being flown more often. In the future, having the total number of flights per manufacturer would increase the robustness of this analysis to more accurately paint a picture of airplane accident statistics.

Now onto our findings.

Boeing had the largest total number of accidents as well as the most total fatalities from 2008-2022. Airbus was the runner up for largest total number of accidents, while Ilyushin was the runner up for total number of fatalities (Airbus followed Ilyushin for total fatalities). The fact that Boeing and Airbus have high numbers of accidents and fatalities does not necessarily seem out of the ordinary when you account for them being the top two biggest plane manufacturers in the world. However, Ilyushin does not even make the top 10 biggest plane manufacturers, making this potentially anomalous. Further, in recent years, the total number of accidents has been at a low for the 2008-2022 time period across all plane manufacturers but specifically for Boeing as well. As the database is updated, we will be able to see if accidents have spiked comparatively in 2023/2024 (which would support media perception of Boeing). Furthermore, the vast majority of airplane accidents appear to be caused by runway safety risks while the majority of airplane accidents leading to fatalities were caused by loss of control in-flight risk. Finally, the majority of accidents and fatalities were in jet-engine type aircraft.