---
layout: post
category: style
tags: [congressional hearings, data, government]
---
{% include JB/setup %}

  I've been running a scraper to collect the
congressional hearings.  This is a public dataset available on
[gpo.gov](http://www.gpo.gov/fdsys/browse/collection.action?collectionCode=CHRG). These hearings are held by
congressional committees 
to discuss current legislation, investigate government activities,
or simply explore a topic of interest. 

  I became aware of this dataset after scraping the presidential remarks
from the GPO site for my previous job [@luckysort](luckysort.com),
a text analytics company in Portland, OR.  When I saw the
hearings dataset, I recalled Stephen Colbert's expert testimony for [House Hearing, 111th Congress - Protecting America's
Harvest](http://www.gpo.gov/fdsys/pkg/CHRG-111hhrg58410/html/CHRG-111hhrg58410.htm). 
His testimony made me curious about the witnesses that congress
frequently bring to speak at these hearings. I started to wonder about
their affiliation with the committee, committee
members, and topic of discussion.
Are they academics? Do they represent a corporate interest? etc. 

  The dataset ended up being 66gb including the text, metadata, and
pdfs. It covers the 99th-102th Congress (1985-2012).  The 99th-104th
Congress appear to be less complete than the later ones. It took about two weeks to collect, primarily due to frequent
timeouts and possibly ratelimiting from the gpo end.  My primary
interest is with the plain text data; I plan to employ natural
language processing algorithms, such as entity extraction, to analyze
the corpus. At some point, I may extract the graphics that are only available in the
pdf to include in an interface.

  For my first pass on the dataset, I plan to index the documents by entities they contain (e.g. corporations, senators, witnesses, etc). The first interface will probably just be a simple search
engine. For my second iteration, however, I would like to incorporate other datasets, like campaign finance data,
and start doing network visualizations.  Or perhaps simply extract network
relationships within the corpus.  This idea will probably evolve as I
work on the first part.  

  Feel free to send me ideas or things you would like to see done.
Also, I might try to sell analytics or even the
api-friendly versions of the raw data on some data platform or just
independently. Contact me if you want to know more. (My email can be
found on my [resume]( hanelifou.com/resume).)  More updates to come!

