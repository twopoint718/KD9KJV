---
layout: page
title: Morse Code
permalink: /morse/
---

I’m learning morse code using the Koch method ~15 wpm I’ll keep this chart updated with my progress.

As a more recent addition, I've enrolled in [CW Academy](https://cwops.org/cw-academy-2/cw-academy/) at Level 1 (total
n00b).
The class starts April 1, 2019.
I will also post updates about that as it goes.
Hopefully my slight efforts here will at least give me a _tiny_ boost ;)
Yeah, right.

{% assign image_files = site.static_files | where: "morse", true %}
{% for myimage in image_files %}
  <img src="{{ myimage.path }}" />
{% endfor %}
