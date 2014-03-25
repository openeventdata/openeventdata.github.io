---
layout: page
title: The Open Event Data Alliance
---
{% include JB/setup %}

This is the Github landing page for the [Open Event Data Alliance](https://github.com/openeventdata). The goal 
of the OEDA is to enable the generation and sharing of open, replicable event
data generated from news sources. Towards this end, we have developed a series
of software tools to achieve this primary goal. For more information about OEDA,
please visit the [homepage](http://openeventdata.org/). Further information
regarding the software tools is outlined below. Finally, information on event
data more generally can be found on the [Computational Event Data System](http://eventdata.parusanalytics.com/)
website.

#Software

###EL:DIABLO

Event/Location: Dataset In A Box, Linux-Option or event data in a box,
basically. EL:DIABLO is a [Vagrant](https://www.vagrantup.com/) box that
enables the easy creation of a virtual machine on the end-user's machine. The
hope is that this box will allow others to easily replicate the same system we
use to generate event data. This will allow others to examine, critique, and
improve upon this system. 

More information can be found at
[http://openeventdata.github.io/eldiablo/](http://openeventdata.github.io/eldiablo/).

###PETRARCH

PETRARCH is the Python-language successor to the
[TABARI](http://eventdata.parusanalytics.com/software.dir/tabari.html) event
data coding software. PETRARCH makes use of a full parse, based on StanfordNLP,
to better perform word disambiguation and noun and verb phrase chunking. This
full parse allows for more accurate event coding. PETRARCH is currently under
active development, and we aim for a full release within the coming months.

More information can be found at
[https://github.com/openeventdata/PETRARCH-Development](https://github.com/openeventdata/PETRARCH-Development).

###Scraper

We make use of a web scraper with a whitelist of RSS feeds to pull news stories
from 166 unique websites. These scraped stories are stored in a MongoDB
database for easy future retrieval. 

More information can be found at [https://github.com/openeventdata/scraper](https://github.com/openeventdata/scraper).

###Pipeline

The pipeline is what moves from the web scraper, through the event coder, and
finally to coded event data. In short, the pipeline is the glue that holds all
of the various components together. 

More information can be found at
[https://github.com/openeventdata/phoenix_pipeline](https://github.com/openeventdata/phoenix_pipeline).
