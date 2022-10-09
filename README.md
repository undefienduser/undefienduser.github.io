{% assign today = site.time | date: '%s' %}
{% assign start = '20-01-2014 04:00:00' | date: '%s' %}
{% assign secondsSince = today | minus: start %}
{% assign hoursSince = secondsSince | divided_by: 60 | divided_by: 60     %}
{% assign daysSince = hoursSince | divided_by: 24  %}

Hours: {{hoursSince}}
Days: {{daysSince}}
