---
layout: post
category: style
tags: [congressional hearings, data, government]
---
{% include JB/setup %}

  For the past two weeks, I've been running a scraper to collect the
congressional hearings.  This is a public dataset available on
[gpo.gov](http://www.gpo.gov/fdsys/browse/collection.action?collectionCode=CHRG). These hearings are held by
congressional committees 
to discuss current legislation, investigate government activities,
or simply explore a topic of interest. 

  I became aware of this dataset after scraping the presidential remarks
from the GPO site for my previous job [@luckysort](luckysort.com),
a text analytics company in Portland, OR.  When I saw the
dataset, I recalled Stephen Colbert's expert testimony to [House Hearing, 111th Congress - Protecting America's
Harvest](http://www.gpo.gov/fdsys/pkg/CHRG-111hhrg58410/html/CHRG-111hhrg58410.htm). 
His testimony gave me the impression that many of the expert
witnesses appear by invitation from members of congress. That in mind,
I started wondering about these witnesses and the types of testimonies
they provide. What is their affiliation with the committee, committee
members, and topic of discussion?
Are they academics? Do they represent a corporate interest? etc. 

  Having worked with standard language processing techniques, this
seemed like an opportune time to use entity extraction on the
corpus. For my first pass on the dataset, I'm working on indexing the documents by entity and
putting a search engine on top of it.  For my second iteration, I
would like to incorporate other datasets, like campaign finance data,
and start doing network visualizations.  Or perhaps simply extract network
relationships within the corpus.  This idea will probably evolve as I
work on the first part.  

  Feel free to send me ideas or things you would like to see done.
Also, I might try to sell analytics or even the
api-friendly versions of the raw data on some data platform or just
independently. Contact me if you want to know more. (My email can be
found on my [resume]( hanelifou.com/resume).)  More updates to come!

