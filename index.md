---
layout: page
title: The Open Event Data Alliance
---
{% include JB/setup %}

This is the homepage of the [Open Event Data Alliance](https://github.com/openeventdata). We turn news into events in a replicable, transparent manner using the [phoenix pipeline](https://github.com/openeventdata/phoenix_pipeline), which relies on a [scraper](https://github.com/openeventdata/scraper), and [TABARI](http://eventdata.parusanalytics.com/software.dir/tabari.html). We are currently working on a successor to TABARI called [PETRARCH](https://github.com/openeventdata/PETRARCH-Development). We are also working on making event data more accessible and transparent by providing virtual machines (via [Vagrant](http://www.vagrantup.com/)) with all the necessary software. You can find more information in each project's repository.

Information on event data more generally can be found on the [Computational Event Data System
](http://eventdata.parusanalytics.com/) website.
    
## Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
