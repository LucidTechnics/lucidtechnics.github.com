---
layout: article
title: Open Data
abstract: Creating open data stores within your organization is the key to increasing data discovery and reuse.
author_twitter: lucidtechnics
author: Bediako George
categories:
- articles
published: true
---


---

When Vivek Kundra was the CIO of the District of Columbia, he championed the idea of a more open government. His thought was that by making the District's data more open, both DC's government and its citizens would inexorably benefit from this in unpredictable ways.

One of the many data opening initiatives he encouraged was Apps For Democracy. This was a project that encouraged private citizens to explore opportunities to mash up government data in ways not thought of by the District itself. The purpose of this project was to provoke a few thoughtful responses from the crowd of application developers with free time to engage in such pursuits.

In just over a month, Apps For Democracy received 47 useful data mash up applications. Why was this so successful?

We think it was successful simply because the District data was made accessible to people who cared about it. And the people who cared about the data did what they wanted to do with it. We call this approach, "The Client Knows Best". Give the client access to the raw data, get out of the way, and watch them produce what they want!

What would happen if this was done in the enterprise? Our own observation is that large corporations do the opposite. Data is not even made fully open to the members of the organization itself. For various reasons, enterprise information is usually trapped within the systems of the business pillars that make up the organization. When these data sets were first established, little or no thought was given towards sharing this information with other departmental groups. Later, when it became apparent that data sharing would be a good thing to have, attempts to make the data more accessible are hamstrung by the initial lack of forethought.

Complicating this is a tendency to "over own" the data. This desire to control the presentation is understandable, but many times the old fashioned mechanisms for achieving data ownership are so restrictive, the consumers of the data are unable to get what they want in a timely fashion. If data is not open, this will always be true!

What do we mean by open data? Well, open data does not mean data that is available to anyone. It is to be expected that some data should not be shared with everyone due to privacy and other concerns; it is also expected, that for an individual that is deemed privy to a data set, the information should gracefully be made available to that individual. How do you accomplish this? Here is what we think the minimum requirements a data store must meet in order for it to be considered open.

* Published data taxonomy - The data's categorical structure shall be made readily apparent to prospective users.
* Robust search capabilities - A user of this data shall be able to perform free text queries against the data store.
* Fundamental CRUD operations - Reading data is fundamental, and so is creating, updating and deleting data. Provided the security credentials of the data user checks out, these functions shall be readily available.
* Change notification - Users of the data store shall have an avenue to understand how the data they have accessed has changed over time.
* Centralized but portable data production rules - Other enterprise systems shall have the ability to create and manipulate new data resources outside of the system of record. Strange as this may sound, enabling other systems to create resources outside of the system of record can result in large magnitude improvements in reliability. This shall be encouraged as long as consumers always consider the data sources system of record to be the single source of truth. It is expected that data resources created in this manner shall eventually be synchronized to its system of record. 

Many data stores in large organizations consistently fall short of these goals. As a point of fact, we have never witnessed a departmental data store that had all these criteria met. This functionality is never built in from the inception. This is a shame, since the truth of the matter is that such functionality is actually quite easy to provide up front.

Our code generation suite Hannibal makes it really easy to have this from the inception. Hannibal allows developers to generate code that performs search, CRUD operations, and change notification out of the box. Furthermore, developers can stipulate declarative security rules that govern who is allowed to view this information. Finally, it makes all of this available via restful web services, so that applications from mainframe processes to desktop browsers can effortlessly access this data as well.

Now your data is open.