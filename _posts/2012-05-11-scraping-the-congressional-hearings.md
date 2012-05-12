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

  The dataset ended up being 66gb including the text, metadata, and
pdfs.  I'm primarily interested in the text data and plan on using
standard language processing algorithms to analyze it.  The
hearings frequently include graphics that are only available in the
pdf, so I decided to go ahead and grab that in case I want to use it
in an interface later.  

  For my first pass on the dataset, I plan on using entity extraction
to grab words of interest, and then I'll index the documents with the
results. The first interface will probably just be a simple search
engine. For my second iteration, I would like to incorporate other datasets, like campaign finance data,
and start doing network visualizations.  Or perhaps simply extract network
relationships within the corpus.  This idea will probably evolve as I
work on the first part.  

  Feel free to send me ideas or things you would like to see done.
Also, I might try to sell analytics or even the
api-friendly versions of the raw data on some data platform or just
independently. Contact me if you want to know more. (My email can be
found on my [resume]( hanelifou.com/resume).)  More updates to come!

