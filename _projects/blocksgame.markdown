---
layout: project
title:  "BlocksGame"
date:   2017-01-05 15:09:49 -0500
categories: jekyll update
---

This is one of my early projects. I used python's turtle graphics to make a fun [BlocksGame][BlocksGame-github].

[BlocksGame-github]: https://github.com/Kcarter787/BlocksGame

{% highlight python %}
def draw_square(t, sq_x, sq_y, sq_size, color = "#33cc33" ):
  """Draws the player square"""
  t.color(color)
  t.begin_fill()
  t.up()
  t.goto(sq_x, sq_y)
  t.setheading(0)  #Face right
  t.down()
  for side in range(4):
    t.forward(sq_size)
    t.right(90)
  t.end_fill()
{% endhighlight %}
