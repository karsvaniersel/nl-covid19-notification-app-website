---
layout: default
title: COVID-19 Notificatie App Status
lang: nl
lang-ref: covid19-notification-app-status-index
---
<p>Hier geven we graag uitleg over de vragen en status van de app</p>

{% assign features = site.features | where:"lang", page.lang %}
{% for feature in features %}
<details class="{{ feature.status }}">
    <summary>
        <h2>{{ feature.title }}</h2>
        <span>{{ feature.summary }}</span>
    </summary>
    {{ feature.content }}
</details>
{% endfor %}