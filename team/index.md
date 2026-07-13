---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

We have a large team of researchers eager to push the limits of AI. Many of our students publish their projects at top venues, and go on to have wonderful research career. Current team members are: 

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'pi'" %}
{% include list.html data="members" component="portrait" filter="role != 'pi'" %}

{% include section.html background="images/background.jpg" dark=true %}

# Alumni

{% include section.html %}

{% include list.html data="alumni" component="portrait" %}
