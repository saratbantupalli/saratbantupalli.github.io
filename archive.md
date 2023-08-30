---
layout: page
title: Blog 
---

{% include base_path %}

{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}

#{% for tag in site.tags %}
  #<h3>{{ tag[0] }}</h3>
  #<ul>
    #{% for post in tag[1] %}
      #<li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    #{% endfor %}
  #</ul>
#{% endfor %}



# layout: archive
# permalink: /archive/
# author_profile: true
# ---

# {% include base_path %}

# {% for post in site.posts %}
#   {% include archive-single.html %}
# {% endfor %}
