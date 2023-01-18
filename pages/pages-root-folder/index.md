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

**This is the page for the winter 2023 edition of the course.**

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

**If Google Calendar preview doesn't work, use the direct link to the [CSE 15L Winter 2023 Calendar](https://calendar.google.com/calendar/embed?src=c_de29a534b0fd24f875f64582371383ec4456898435a842b7b554ceb65c8388b3%40group.calendar.google.com&ctz=America%2FLos_Angeles).**

<iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=1&bgcolor=%23ffffff&ctz=America%2FLos_Angeles&mode=WEEK&showPrint=1&showCalendars=0&src=Y19kZTI5YTUzNGIwZmQyNGY4NzVmNjQ1ODIzNzEzODNlYzQ0NTY4OTg0MzVhODQyYjdiNTU0Y2ViNjVjODM4OGIzQGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20&color=%23B39DDB" style="border:solid 1px #777" width="800" height="600" frameborder="0" scrolling="no"></iframe>

## Frequently Asked Questions

**Q: I'm also taking Math 18, or some other course whose final exam time
overlaps with CSE15L. What should I do?**

We will have scheduled oral exams in CSE15L with appointment slots.  If you
don't have the time of the final exam free due to a conflict, you just need to
be flexible in scheduling your exam some time during finals week.

**Q: Will the course have remote options?**

No. Plan to attend all lecture and lab sessions in person. Participation
policies will take into account that not all students can make it all the time,
but we will not have remote equivalents for completing lab and lecture.

**Q: Is participation required?**

Yes. A final policy will be posted by the start of the quarter with details,
but you should plan to attend both lecture and your assigned lab section every
week.

**Q: I have a question about enrollment or the waitlist.**

Check the web registration across all the sections; the course has 14 separate
lab sections, and their enrollments and waitlists are independent and
fluctuate. Contact [CSE
Advising](https://cse.ucsd.edu/undergraduate/undergraduate-advising) for more
information on enrollment and waitlist processes.

**Q: How should I prepare for the course?**

Review Java (for example, [CSE11](https://ucsd-cse11-f21.github.io/)). Check
out some related resources like [MIT missing
semester](https://missing.csail.mit.edu/). Get enough sleep and set up your
schedule so you can make the class and lab times. Bookmark this web site! 
