---
layout: project
title:  "BlocksGame"
date:   2016-01-05 15:09:49 -0500
categories: jekyll update
---

This is one of my early projects. I used python's turtle graphics to make a fun [BlocksGame][BlocksGame-github].

[BlocksGame-github]: https://github.com/Kcarter787/BlocksGame
My natural intuition when I started building this project was to partition up the tasks into what I thought made logical sense.
For example, one method is responsible for drawing the player-controlled block with a particular size and location.
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
Not having studied computer science, I actually wasn't aware that I was using an important technique called abstraction.
