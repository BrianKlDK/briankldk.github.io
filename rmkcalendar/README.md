# What
Convert iCalendar ics to [FullCalendar][0] json using [ical.js][1].

## Usage
- Edit `js/custom_display.js` to provide your ics feed(s) and colors.

**important:** ensure you provide sufficient CORS access on the web server hosting the ics feed(s) or nothing will display (visible in browser console).

# Why
Because it's so much better to sync your website calendar with ics feed(s) that you can edit from wherever than having to handle that within an admin webpage.

# How
This all came from [https://github.com/leonaard/icalendar2fullcalendar](https://github.com/leonaard/icalendar2fullcalendar), which provides an out-of-the-box working solution to view calendar(s) from ics URL feeds using fullcalendar.

We 'built' (horribly hacky, but works) on that to obtain a calendar that also shows descriptions for events and handles better output info for full days event (which is already implemented in fullcalendar but somewhat not always detecting such events) and multiple days-spanning event. Most of the additional code is in `js/custom_display.js` and this is the only file you need to edit to adjust this project to your needs.

## Dependencies
A whole lot of JS stuff (in ./js/). Since newer versions are very likely to break code and I'm a JS noob, 
librairies used for this project are all inside the repo. Feel free to update the code for more
recent versions and queue in a nice Merge Request afterwards.


# Contribute
PRs welcome of course, especially to provide compatibility with more recent versions of FullCalendar.io

[0]: http://fullcalendar.io/
[1]: https://mozilla-comm.github.io/ical.js/
