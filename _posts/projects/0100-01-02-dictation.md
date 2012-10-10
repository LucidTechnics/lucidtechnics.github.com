---
layout: project
title: Dictation
abstract: ... an open source english based domain specific language for describing business applications.
prose_link:
  http://prose.io/#lucidtechnics/lucidtechnics.github.com/edit/master/_posts/features/0100-01-02-dictation.md
author_twitter: lucidtechnics
author: Bediako George
image: /images/nature.jpeg
categories:
- projects
published: true
---

Dictation is an open source english based domain specific language for describing business applications.  Using Dictation, one can describe all resources in your business environment, then take that description and generate working software from it.  This is the method we use to rapidly build your software.  Dictation can describe your business down to the lowest levels, even including your operation's audit and security concerns.

The best thing about Dictation is how easy it is to read and write. Our less technically savvy clients can fully understand Dictation.  It looks and sounds just like english!  Take a look at the following example of Dictation paragraphs that describe a customer, her order, and the line items in the order.

    A Customer
    has a nick name
    has a full name
    has a date of birth (dictation automatically knows this has the type "date")
    has a social security number which is sensitive
    can be viewed or created or changed by a customer service representative

    An Order
    belongs to a Customer
    has a description
    can be viewed or created or changed by a customer service representative

    An Order Line Item is audited (lets dictation know to keep track of all changes)
    belongs to an Order
    has a description
    has a price which is a number
    can be viewed or created or changed by a customer service representative

After describing your business using Dictation requirements as shown above, we can then generate software that will support a fully function order taking application.