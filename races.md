---
layout: default
title: Charlottesville Racing Club Races
permalink: /races/
---

## Races


### Club-sponsored races
The Charlottesville Racing Club organizes several races each year in a number of disciplines.

{% for race in site.data.races %}
<div class="row section">
    <div class="col-md-3 text-center">
        {% if race.image %}
            {%if race.bikereg %}
            <a href="{{race.bikereg}}">
                <img src="{{site.baseurl}}/images/{{race.image}}" alt="{{race.name}} Image" class="block-image"/>
            </a>
            {% else %}
            <img src="{{site.baseurl}}/images/{{race.image}}" alt="{{race.name}} Image" class="block-image"/>
            {% endif %}
        
        {% endif %}        
    </div>
    <div class="col-md-9">
        <h4>
            {% if race.id %}
                <a href="{{race.id}}">{{race.name}}</a>
            {% else %}
                {{race.name}}
            {% endif %}
        </h4>
        {% if race.date %}
            <p>{{race.date}}</p>
        {% endif %}
        {% if race.bikereg %}
            <p><strong>Register:</strong> <a href="{{race.bikereg}}">{{race.bikereg}}</a></p>
        {% endif %}
        <p>{{race.desc}}</p>
    </div>
</div>
{% endfor %}

### Other races
CRC participates in races in a wide variety of disciplines. Many of these events can be found on Bikereg.com, although some disciplines have specific calendars maintained by other regional cycling organizations.
