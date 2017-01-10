---
layout: project
title:  "TaskCat"
date:   2017-01-06 15:09:49 -0500
categories: jekyll update
---
[TaskCat][TaskCat-github] is a program that helps you keep track of your time.

[TaskCat-github]: https://github.com/Kcarter787/taskCat


{% include projects_image.html name="task_cat.png" caption="TaskCat makes sure you manage your time" %}

{% include projects_image.html name="taskcat_report.png" caption="TaskCat makes sure you manage your time" %}

{% highlight python %}
# Specify a name and ext for your data
FILE_NAME = "task_log"
FILE_FORMAT = ".csv"

class taskEntry():
    def __init__(self, description, time_estimate):
        self.description = description
        self.time_estimate = time_estimate
        self.note = None

    def mark_start_time(self):
        self.time_started, self.time_started_str, self.time_started_abs = \
            time.localtime(), time.ctime(), time.time()

    def mark_end_time(self):
        self.time_finished, self.time_finished_str, self.time_finished_abs = \
            time.localtime(), time.ctime(), time.time()
{% endhighlight %}

This is empty for now
