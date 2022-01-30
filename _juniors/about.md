---
layout: default
title: About
order: 1
id: about
permalink: /juniors/about/
---

## About the Junior Mountain Bike Team

[[image here]]

The Charlottesville Racing Club/Blue Ridge Cyclery Junior MTB team is a co‐ed development mountain 
bike team based in Charlottesville for youth ages 8 through 18. The team is open to youth from 
around the region with skill levels ranging from beginners who ride and learn skills with our 
junior development team, to our JV team, all the way up to our varsity team that trains and races 
at the highest level. The team focuses on developing age-appropriate MTB skills in a fun, safe, and supportive environment. 

The team is the junior division of the Charlottesville Racing Club, a local ride club that is committed 
to promoting youth cycling within the larger group of cyclists which includes triathletes, road racers, 
mountain bike racers, and folks who ride for fun. The team is made possible by our sponsors including 
main sponsors [Blue Ridge Cyclery](https://www.blueridgecyclery.com/) and [Reynolds GM-Subaru](https://www.reynoldsgmsubaru.com/).

For more information see the following pages:

<ul>
{% for page in site.juniors %}
{% assign sorted = site.juniors | sort:"order" %}
    {% if page.order > 1  %}
        <li>
            <a href="{{page.id}}">{{page.title}}</a>
        </li>
    {% endif %}
{% endfor %}
</ul>
