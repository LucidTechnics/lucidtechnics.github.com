---
layout: project
title: Dictation
abstract: ... an open source english based domain specific language for describing business applications.
prose_link:
  http://prose.io/#lucidtechnics/lucidtechnics.github.com/edit/master/_posts/features/0100-01-02-dictation.md
author_twitter: lucidtechnics
author: Bediako George
image: /images/typewriter_800_352.jpg
categories:
- projects
published: true
---

Dictation is an open source english based language for describing business applications.  Using Dictation, one can describe in plain english how your business works.  We can then take that description and rapidly generate working software from it.  Dictation can describe your business down to the lowest levels, even including your operation's audit and security concerns.

![Washington DC train status electronic sign](https://raw.github.com/LucidTechnics/lucidtechnics.github.com/master/images/typewriter_600_282.jpg)

The best thing about Dictation is how easy it is to read and write. You do not have to be technically savvy to fully understand Dictation.  It looks and sounds just like plain english!  Take a look at the following example of Dictation paragraphs that describe a customer, her order, and the line items in the order.

    A Customer
    has a nick name
    has a full name
    has a date of birth
    has a social security number which is sensitive
    can be viewed or created or changed by a customer service representative

    An Order
    belongs to a Customer
    has a description
    can be viewed or created or changed by a customer service representative

    An Order Line Item is audited
    belongs to an Order
    has a description
    has a price which is a number
    can be viewed or created or changed by a customer service representative

After describing your business using Dictation requirements as shown above, we can then generate software that will support a fully functional order taking application.  The generated software will understand that customers have orders, orders have line items, and that any changes to an order's line items should be recorded.  Also the software will automatically encrypt the customer's social security number as it is deemed to be sensitive information.

We estimate that using Dictation along with <a href="http://lucidtechnics.github.com/projects/airlift.html">Airlift</a>, our open source cloud based web application framework, we can reduce a typical web application project's execution time by 50% or more.