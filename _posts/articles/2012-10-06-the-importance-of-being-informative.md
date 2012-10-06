---
layout: article
title: The Importance of Being Informative
abstract: ... how can Washington D.C. metro system do a better job of communicating train status using their existing electronic signs?
author_twitter: _mql
author: Bediako George
categories:
- articles
---

If you are a public transit commuter in Washington D.C., no doubt you are spending a fair portion of your time wondering about the state of our subway transit. I have been commuting via subway for a fair number of years now, and during that time I have often made observations about the dynamics of our subway, and how they relate to the design and architecture of applications that we build for the web.

It was not so long ago that WMATA installed status signs above the tracks in every subway station. As an example, I have included a photo of one of those signs.

This represents a big improvement over what had existed before, which was limited to a set of flashing lights at track level meant to warn you that a train was just arriving, but really nothing more than that. Without these signs, passengers would stand in the subway station without any clue as to when the next train will arrive.

As you can see the color of the line (RED), the size of the train in cars (6), the direction (GLENMONT) and the arrival time (ARR) is presented on these status signs. This is a good thing because it helps newly arriving customers that enter the train station understand how long they have to wait before their train arrives.

But I submit that this is not good enough. As a matter of fact, with just a little more thought metro could have done much better. Here are all the things I think are actually wrong with the current implementation:

1. These electronic dynamic signs are being used to present mostly static information. Over half of the sign is used to present the name of the line (RD) and the direction of the train (GLENMONT), but for a given platform on our subway this never really changes! The train station is littered with signs that tell you the direction of the train on the track, and the train itself tells you the final station so having this information on a electronic sign is pretty much redundant. Displaying static information is not the best way to use a dynamic presentation sign.
2. Although the "next train arriving information" is certainly relevant, it is not the most pertinent to a metro traveller. The status signs tell you how long you have to wait until the next car arrives, but is this really what you want to know? Or is there something more pertinent than this?
3. The signs are in the wrong location. These signs provide important information about the state of the system, yet they are located far inside the metro. In most stations, most of these signs are not even visible from the areas where customers may purchase tickets.

So how could this have been done better? Well, let us look at the relevance issue first. My observation is that although the next train arriving information is good to have, I think what I really care about is when will I arrive at my destination? When I arrive at a given metro station I would want to know if the system is performing at peak capability for the route I want to travel on. These signs actually give the traveler information that is really only important from the WMATA's point of view and not from the passenger's own standpoint.

So what would be a good way to represent this? What I am suggesting looks very much like the flight status boards you see in modern airport terminals, except instead of displaying departure times for trains leaving the station it should show the expected arrival times for all the stations in the system accessible from this track (direction) at this station.

And finally, the last change I would suggest is to make these signs viewable from the street entrances. Why? As a traveler I want to know the state of metro before I pay my fare. I should be able to decide whether or not I want to ride the train, take a taxi, or drive to my destination. This is very important because open systems with finite capacity (like subways and highways) cannot control the arrival patterns of new users. As a matter of course, systems like these should always provide real time performance capability feedback to its end users. In the case of Washington DC's subway, this would allow the system to recover from performance issues more gracefully. When the system is overloaded, some customers would not enter the train station if they were made aware of issues at the gate. Taxi cab drivers will also be able to use this information to pick up passengers that, due to the current overloaded state of the subway system, would not want to rely on metro to get them to their destinations on time.

I have addressed the three aforementioned issues, but there is still one issue that I have not handled. It is a matter of money. Metro has already invested quite a bit of money on the signs they have, and money in this climate is hard to find. How could WMATA implement the improvements I am suggesting at minimal cost to the taxpayers of DC?

Well, one way to do this would be to reuse the existing signs. There is a problem with this approach. The Washington DC metro has over 80 metro stations. To show all 80 of those stations using the existing status boards would be a challenge to say the least. How could we present this amount information given such a limitation in real estate?

What if WMATA used colored symbols (shapes) combined with a prioritized information set? One example of such a presentation could be to model this using a combination of popular station hops and system status colors. The picture below gives you an example of what one such sign would look like:

So instead of showing the end of the line information and the arrival time of the next train, we can show the expected arrival times for key stations in the system. What stations would qualify as key stations? This would depend on the station you are waiting in, but it would most often be transfer stations, and popular exit points. So if you get on the Red line train at Takoma station and you are heading downtown during the morning rush hour, the message board should give you the expected arrival times for Takoma, Union Station, Gallery Place, and Metro Center. For the vast number of travelers entering Takoma I would expect that this would be more than enough to determine whether or not the system is working well. The color coded symbols will tell you whether or not the expected arrival time is considered normal or abnormal.

In the sign above, the 7 minute delay between Gallery Place and Metro Center is considered below normal performance, and as such, a red heptagon (for color blind people a change in shape is helpful) indicates that the system is performing below expectations between Gallery Place and Metro Center.

In many ways, the information sharing challenges experienced by Washington DC's metro system are similar to many of the issues we architects experience in creating high performance web sites. Displaying accurate system status to end users is a design factor too often left out. This blog posting addresses this mistake in a highly used and very public transit system but the techniques used to solve those problems can be directly transfered to similar situations on the Web.