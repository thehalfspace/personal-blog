---
title:  "Predicting Earthquakes"
subtitle: "Where are we?"
date: 2020-12-27T23:49:25+05:30
comments: true
keywords: []
tags: [misc.]
draft: false
toc: false
---


```I am taking a course on communicating your science in Winter 2018 and this post is a part of the assignment. I will try to continue writing more stuff like this.```

Are we having big earthquakes more often these days compared to the past? 

 If we look at [the data](https://earthquake.usgs.gov/earthquakes/browse/largest-world.php), the answer seems to be yes: a lot of big events happened after the year 2000! Most big earthquakes occur at the interface of continent and ocean boundaries, and therefore are usually followed by a series of tsunamis just as devastating as the earthquakes themselves. For example, the Sumatra-Andaman earthquake of 2004 was the third largest event ever recorded on modern instruments and it was the longest lasting earthquake ever observed, lasting upto 10 minutes. A series of devastating tsunamis followed, killing more than 220,000 people in 14 countries, and the combined damage was the most ever recorded. The Tohoku earthquake of 2011 near the coast of Japan and the associated tsunami claimed nearly 16,000 lives, and was the fourth most powerful event recorded on the earth. The Nepal earthquake of 2015 was one of the worst natural disaster to strike Nepal, claiming nearly 8000 lives. The largest earthquake ever recorded was the Great Chilean Earthquake of 1960, with a magnitude of 9.5, but a lot of the above mentioned earthquakes were much more damaging owing to the local geology and the population density of the region. To get an idea of how damaging these events are, the Sumatra-Andaman earthquake tremor was so strong that it wobbled the earth's rotation axis by almost an inch.   
 
Most people are familiar with these earthquakes from news sources, but these sources often fail to recognize that all of these "really big" events happened after the year 2000. Now, if we think back to the period between 1960-2000, we wouldn't recall this many big earthquakes. Look at the data again for confirmation. This recent increase in the number of large earthquakes have garnered concerns that the rate of earthquake activity has increased significantly, which would have important implications for hazard mitigation.

Understanding trends in earthquakes is not only important because it can help society be prepared for effective hazard mitigation, but also because any evidence of non-randomness in the observed earthquake data would give us hope that earthquake prediction, to a certain extent, might be possible. On the other hand, an inherent randomness in the set of observations would suggest that there is no basis for prediction.

Earthquake prediction is one of the most fundamental challenges in the earth sciences. The reason for lack of progress in this direction is attributed to lack of direct observations of earthquakes, since they happen at depths we can't reach. As an analogy, weather and climate systems are just as complex as earthquakes, if not more. But the only reason we can attempt an effictive weather forecast is that the system is directly observable. To understand earthquakes, scientists usually look at the movement of ground on the surface of the earth, and try to extract the information at depths from this surface movement. Here, we attempt to find a pattern in the sequence of big earthquakes, i.e., we address the question: do the big earthquakes contain any information about the next one? Finally, we will look at some of the existing strategies to minimize damage from a big earthquake, and how can we move forward.

To look at the pattern of earthquakes, we can generate a series of random numbers in space and time constrained by the earthquake properties (Magnitude and Frequency), such that it mimics the sequence of earthquakes in the real earth. We call this set of earthquakes an earthquake catalogue. We generate a large number of such catalogues randomly, and look at how many of them are in agreement with reality. We would ideally generate around a million of such catalogues, and look at how many earthquakes greater than Magnitude 7 happen within the time period of 2000-2018.  If a significant number of the catalogues agree with reality, the earthquake sequences are indeed random. On the other hand, any apparent anomaly in the real observations would not be reflected in the random catalogues, and would suggest an underlying pattern in the earthquake sequences. [A systematic study](http://www.pnas.org/content/pnas/109/3/717.full.pdf) was performed by scientists in California based on this idea, and they came to a conclusion that the sequence of large earthquakes is not distinguishable from an equivalent random process. Thus, the global risk of earthquakes today is no higher than it has been in the past. I tried to do a [similar exercise](https://github.com/thehalfspace/coursework/blob/master/Global_earthquake_randomness.pdf) as the study above with more recent dataset, and reached similar conclusions.

This leads us to a grim conclusion that there is no correlation between two large earthquakes, that is, one large earthquake happening today does not tell us about the next large one in any way. 

Now what? 

Should we give up?

Of course not! While there is less hope for a long-term prediction (think decades or centuries), a lot of things can be done over shorter time periods (think seconds and minutes). If an earthquake strikes our home, it does a lot more than just violent ground shaking. Earthquakes can lead to more destructive secondary hazards, like tsunamis, forest fires, or rock slides. An earthquake in California rupturing a gas pipeline could be a potential fire hazard. As we have seen above, a tsunami due to an earthquake claims a lot of lives. Thus, the knowledge of earthquakes even a few minutes prior to the destruction becomes imperative. Luckily, earthquake waves travel through earth in different phases. A direct, less destructive wave traveling through the volume of the earth arrives before the more destructive waves traveling along the surface of the earth. This gives us around a few minutes between the detection of an earthquake and the onset of destruction. While this is the best we can do for now, it is enough for a person to place themselves out of immediate danger. More importantly, we would have sufficient time to shut down a city's power supply, lest the damage to electrical wires result in a fire. Similarly, we would have some time to evacuate people from the coastlines against a tsunami warning. 

Scientists have been working on developing an earthquake early warning system that would alert people few seconds to few minutes before an earthquake, depending on the size of the earthquake. A free app called [ShakeAlert](https://www.shakealert.org/), which is still in the development phase, has seen some success in warning people just before the earthquake could be felt. While countries like Japan and Mexico regularly use texts and siren blares to warn the people, US lags behind, still being in the beta testing mode. Given the past record of earthquakes in the US, a better warning system is a necessity. An earthquake early warning system can give us enough time to slow trains and taxiing planes, prevent cars from entering bridges and tunnels, move away from dangerous machines or work environments, or to evacuate a building.

The past few decades have seen an exponential growth in earthquake research, and the coming decades promise us with a lot more data, therefore now is a good time to delve into understanding earthquakes.

References:
----------
* http://www.pnas.org/content/pnas/109/3/717.full.pdf
* https://www.shakealert.org/


