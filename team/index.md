---
title: Team
nav:
  order: 4
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

AVIS Lab is a group of undergraduate and graduate researchers working with Dr. Md Mehedi Hasan on computer vision, robot learning, and intelligent systems.
Students lead their own projects from first idea to published paper. Recent work has appeared in Findings of ACL, *PLOS One*, *Plant Methods*, *Smart Agricultural Technology*, and *IEEE Access*.
Our alumni have gone on to PhD and MSc programs at the University of Kentucky, the University of Georgia, the University of Central Florida, the University at Albany (SUNY), the University of Dayton, UNC Charlotte, and Mississippi State University, and to AI roles in industry.

Interested in joining? See [Join Us]({{ "/contact/" | relative_url }}).

{% include section.html %}

## Current members

{% include list.html data="members" component="portrait" filter="role == 'principal-investigator'" %}
{% include list.html data="members" component="portrait" filter="role != 'principal-investigator'" %}

{% include section.html background="images/background.jpg" dark=true %}

# Collaborators

{% include section.html %}

Researchers who work with the lab remotely on joint projects.

{% include list.html data="alumni" component="portrait" filter="role == 'collaborator'" %}

{% include section.html background="images/background.jpg" dark=true %}

# Alumni

{% include section.html %}

Former lab members and where they are now.

{% include list.html data="alumni" component="portrait" filter="role == 'alum'" %}
