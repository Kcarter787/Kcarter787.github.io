---
layout: project
title:  "EatUp"
date:   2017-01-05 15:09:49 -0500
categories: jekyll update
---

Check out the [EatUp website][Eatup-site] to learn more!

[Eatup-site]: http://www.eatup-app.com
{% capture includeGuts %}
{% include projects_image.html name="eatup_logo.png" caption="EatUp - an algorithm based iOS app for staying in touch with friends" %}
{% endcapture %}
{{ includeGuts | replace: '    ', ''}}
