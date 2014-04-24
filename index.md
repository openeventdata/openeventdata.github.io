---
layout: page
title: The Open Event Data Alliance Software Page
---
{% include JB/setup %}

This is the Github landing page for the software being developed by the [Open Event Data Alliance](https://github.com/openeventdata). For more information about OEDA,
please visit the [homepage](http://openeventdata.org/). In a nutshell, the goal 
of the OEDA is to enable the generation and sharing of open, replicable event
data generated from news sources. We have developed a series
of software tools to generate event data, which are described below. Information on event
data more generally can be found on the [Computational Event Data System](http://eventdata.parusanalytics.com/)
website.

#Software

###PETRARCH

PETRARCH is the Python-language successor to the
[TABARI](http://eventdata.parusanalytics.com/software.dir/tabari.html) event
data coding software. PETRARCH makes use of a full parse, based on Stanford CoreNLP,
to better perform word disambiguation and noun and verb phrase chunking. This
full parse allows for more accurate event coding. PETRARCH is currently under
active development, and we aim for a full release in the summer of 2014.

More information can be found at
[https://github.com/openeventdata/PETRARCH-Development](https://github.com/openeventdata/PETRARCH-Development).

###[EL:DIABLO](http://openeventdata.github.io/eldiablo/)

Event/Location: Dataset In A Box, Linux-Option or event data in a box,
basically. EL:DIABLO is a [Vagrant](https://www.vagrantup.com/) box that
enables the easy creation of a virtual machine on the end-user's machine containing all the tools needed for generating event data (including the scraper and pipeline described below). Our hope is that this box will allow others to easily replicate the system we use to generate event data. This will allow others to examine, critique, and improve upon our system. 

More information can be found at
[http://openeventdata.github.io/eldiablo/](http://openeventdata.github.io/eldiablo/).
Or go straight to the [repository](http://openeventdata.github.io/eldiablo/).


###[Scraper](http://oeda-scraper.readthedocs.org/en/latest/)

We make use of a web scraper with a whitelist of RSS feeds to pull news stories
from ~160 unique websites. These scraped stories are stored in a MongoDB
database for easy future retrieval. 

More information can be found at
[https://github.com/openeventdata/scraper](https://github.com/openeventdata/scraper)
with documentation at
[http://oeda-scraper.readthedocs.org/en/latest/](http://oeda-scraper.readthedocs.org/en/latest/).

###[Pipeline](http://phoenix-pipeline.readthedocs.org/en/latest/)

The pipeline is what moves from the web scraper, through the event coder, and
finally to coded event data. In short, the pipeline is the glue that holds all
of the various components together. 

More information can be found at
[https://github.com/openeventdata/phoenix_pipeline](https://github.com/openeventdata/phoenix_pipeline)
with documentation at
[http://phoenix-pipeline.readthedocs.org/en/latest/](http://phoenix-pipeline.readthedocs.org/en/latest/).
