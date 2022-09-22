---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: page-fullwidth
header: no

#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
title: "Software Tools & Techniques Lab (UCSD CSE15L)"
---

Joe Gibbs Politz - <code>jpolitz@eng.ucsd.edu</code> -  [jpolitz.github.io](https://jpolitz.github.io)



## Material and Schedule

<ul class="material">
    {% for post in site.categories.week reversed %}
    <li class="{% if post.current %}current{% else %}gray{% endif %}">
    <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    <ul>
      {% for todo in post.todos %}
      <li><a href="{{ todo.url }}">{{ todo.name }}</a> - Due {{ todo.due-date }}</li>
      {% endfor %}
    </ul>
    
    </li>
    {% endfor %}
</ul>

## Course Calendar

This calendar shows rooms for scheduled in-person lecture and lab meetings.

<iframe src="https://calendar.google.com/calendar/embed?src=c_7ci66429f3tppf1qfhijom88m4%40group.calendar.google.com&ctz=America%2FLos_Angeles" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

## Frequently Asked Questions

For now, this page is a placeholder and holds frequently asked questions about
the course. This site will switch to containing the official course website and
syllabus at the start of winter quarter (September 19, 2022).

**Q: Will the course have remote options?**

No. Plan to attend all lecture and lab sessions in person. Participation
policies will take into account that not all students can make it all the time,
but we will not have remote equivalents for completing lab and lecture.

**Q: Is participation required?**

Yes. A final policy will be posted by the start of the quarter with details, but
you should plan to attend both lecture and your assigned lab section every week.

**Q: What about week 0 and Thanksgiving week?**

There will be no official lab sessions in week 0 (because it would only be the
Thursday lab sessions) and no lab on November 23/24. All students will have a
shorter asynchronous activity in those times – in week 0 it will be about
getting set up and in Thanksgiving week it will be about relevant material at
that point in the course.

In-person activities for the course will start as usual in week 1 (September
26).

Lecture on Wednesday, November 23 will be **remote** and
**asynchronous**. There will still be lecture content with associated
*participation, but you can do it any time on the 23rd.

**Q: I have a question about enrollment or the waitlist.**

At this point, the waitlist is processed in first-come, first-serve order – for
each student in the class that drops, a student on the waitlist joins. To get a
spot in the class you should attend lecture and lab and do all the usual course
activities. Check the web registration across all the sections; the course has
10 separate lab sections, and their enrollments and waitlists fluctuate. Contact
[CSE Advising](https://cse.ucsd.edu/undergraduate/undergraduate-advising) for
more information on enrollment and waitlist processes.

**Q: How should I prepare for the course?**

Review Java (for example, [CSE11](https://ucsd-cse11-f21.github.io/)). Get
enough sleep and set up your schedule so you can make the class and lab times.
Bookmark this web site!