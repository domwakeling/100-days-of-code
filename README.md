# 100 Days Of Code - Log

### Day 1: January 2, 2017

**Today's Progress**: Finished 'Rogue(like) Adventure' (Project 15 on
  FreeCodeCamp).

**Thoughts:** Code is a little messy in places and could do with being
re-factored. The dungeon generator (Dungeon class) could be appropriate for
putting out as open-source (or at least posting on GitHub!)

**Link to work:** [Rogue(like) Adventure on CodePen](https://codepen.io/domwakeling/full/ObKvWq/)

### Day 2: January 3, 2017

**Today's Progress**: Started work on FreeCodeCamp Project 16 (Bar
  Chart). Ran through tutorials at Mike Bostock's site
  ([part1 ](https://bost.ocks.org/mike/bar/1) and
  [part 2](https://bost.ocks.org/mike/bar/2)), trialled in CodePen, and added a
  third chart pulling and visualising the FCC-provided JSON set.

**Thoughts:** Know very little about ```<svg>``` elements in HTML, need to do some
additional research on this; seems likely there will be more of this coming up!

### Day 3: January 4, 2017

**Today's Progress**: Finished working on FreeCodeCamp Project 16 (Bar
  Chart). Main changes implemented:

  - added vertical & horizontal axis
  - added vertical scale (requiring reversing of scale domain so that
  the numbers ran true, and necessitating changes to height and transforms for the bars)
  - added horizontal scale
  - added tooltips
  - added title and legend for vertical axis
  - styling including changing colours of axis, tick-marks and scales to match dark background

Primary resources used was the tutorial at Mike Bostock's site
  ([bar chart part 3](https://bost.ocks.org/mike/bar/3)) together with [D3 Tricks & Tips](https://leanpub.com/d3-t-and-t-v4/read) by Malcolm Maclean.

**Thoughts:** Seems like just getting started with D3 (and as noted yesterday, don't really have the background in ```svg```). In the absence of tutorials/challenges at FreeCodeCamp (which I think are coming) have found some other resources which I'll be looking at in coming days to improve knowledge.

**Link to work:** [Bar Chart on CodePen](https://codepen.io/domwakeling/full/XpWpmW/)

### Day 4: January 5, 2017

**Today's Progress**: Finished FreeCodeCamp Project 17 (Scatterplot
  Chart).

**Thoughts:** Remember to check whether SASS/CSS styling of D3 elements is
overwriting styling applied in Javascript - spent half an hour overcoming an
apparent failure  of ```.attr('text-anchor','start')``` only to find that I'd
applied ```'end'``` as part of CSS.

**Link to work:** [Scatterplot Chart on CodePen](https://codepen.io/domwakeling/full/wgBMWb)

### Day 5: January 6, 2017

**Today's Progress**: Finished FreeCodeCamp Project 18 (Heat Map
  Chart).

**Thoughts:** Found a bug where the tooltip temperature expected a number
  (passed to a string) with at least three decimal places and in **one** instance
  the calculated value was **exactly** an integer. Easy-ish to fix once I'd
  worked out what was causing the issue ... but **never asuume**.

**Link to work:** [Heat Map Chart on CodePen](https://codepen.io/domwakeling/full/KawqXJ/)

### Day 6: January 7, 2017

**Today's Progress**: Finished FreeCodeCamp Project 19 (Force Directed
  Chart).

**Thoughts:** Struggled to get flag images showing, eventually realised that
I needed to add the ```<img>```s to an HTML ```<div>``` rather than to
the ```<svg>``` that I was using for the rest of the chart; then give the
absolute positioning to the ```<div>``` and everything worked. Would have preferred
circular flags, but could't find a sprite-map that had square images suitable for this.

**Link to work:** Force Directed Chart on [CodePen](http://codepen.io/domwakeling/full/PWqKPB) and [GitHub](https://github.com/domwakeling/FreeCodeCamp-Project-19)

### Day 7: January 8, 2017

**Today's Progress**: Finished FreeCodeCamp Project 20 (Map Data on Globe).

**Thoughts:** This one was tricky; took a long time to work out how
to get the data to visualize using a globe (really wanted to use a
  spherical view rather than a flattened map) and then get everything
  to move/zoom correctly. Probably spent 3-4 hours trying various
  solutions before I hit on the correct one.

  Also (happilly) have worked out that if I store a data file on
  GitHub and then click on the "RAW" button, I can get a link to
  the original file which WILL work when using various JSONs.

**Link to work:** Global Data & Map on [CodePen](http://codepen.io/domwakeling/full/apvbrO/) and [GitHub](https://github.com/domwakeling/FreeCodeCamp-Project-20)

### Day 8: January 9, 2017

**Today's Progress**: Completed how-to-npm.

### Day 9: January 10, 2017

**Today's Progress**: Started learnyounode

**Thoughts**: Getting a little trickier after a fairly simple introduction to
npm yesterday, node.js is taking a bit more thought. Have finished half the
exercise, starting to expose some of the more "server-y" side of things.

### Day 10: January 11, 2017

**Today's Progress**: More learnyounode - up to (and including) TCP time server.

### Day 11: January 12, 2017

**Today's Progress**: Finished learnyounode.

**Thoughts**: Just when you think it's insanely difficult, it turns out there's
a really simple solution ... and vice versa ...

### Day 12: January 13, 2017

**Today's Progress**: Node and Express

**Thoughts**: Ran through the FreeCodeCamp module on Express, using the 'expressworks' package from Node School. Completed the tutorials.

### Day 13: January 14, 2017

**Today's Progress**: FreeCodeCamp Project 21

**Thoughts**: Project is to create a microservice which is passed **either** a
date (in natural format) **or** a Unix timestamp in it's URL, and to return a
JSON object containing both the timestamp and the natural date.

Got set up with Heroku (limited instructions but not difficult) and
using ```sass-middleware``` in Node. Some hiccups along the way, but nothing
major.

**Link to work:** [Live App](https://dry-castle-31853.herokuapp.com/) on Heroku,
[source code](https://github.com/domwakeling/FreeCodeCamp-Project-21) on GitHub.

### Day 14: January 15, 2017

**Today's Progress**: FreeCodeCamp Project 22

**Thoughts**: Project is to create a microservice which returns a JSON with the
IP address, language and operating system that sent the request. This was
actually a very quick and simple challenge, essentially just had to add
Express as a dependency and write a very short server.js file ...

**Link to work:** [Live App](https://evening-inlet-32614.herokuapp.com/) on Heroku,
[source code](https://github.com/domwakeling/FreeCodeCamp-Project-22) on GitHub.

### Day 15: January 16, 2017

**Today's Progress**: Finished 'learnyoumongo'

**Thoughts**: Note that when using the collection.aggregate function, (a) it needs
to be passed **an array** of match/action objects, and (b) when extracting data
from the ```$match```ed items, the key being used needs to have a $ prefix - so
for instance if you're summing over ```'price'```, you need to ```$sum: '$price'```

### Day 16: January 17, 2017

**Today's Progress**: Experimenting with a D3.js implementation for LSERSA website.

**Thoughts**: Building a GeoJSON file is surprisingly simple, but remember to
invert latitude/longitude when entering geometry coordinates. Working in test
environment at the moment, will send live in due course.

### Day 17: January 18, 2017

**Today's Progress**: Improvements to the D3.js implentation for LSERSA

**Thoughts**: Found a better (world) dataset via
[GitHub](https://github.com/datasets/geo-countries) - note that it's a 24MB file
but by cutting out everything except UK & Rep Ireland it's only 400KB. Also fixed
zoom/pan on the chart (hadn't set ```d3.event.preventDefault()``` as a method).
Some more work to do before putting this live, but principal coding is working well.

### Day 18: January 19, 2017

**Today's Progress**: Working on a new idea - wire-framing a webpage

### Day 19: January 20, 2017

**Today's Progress**: Continuing work on idea - basics finished, info
modal implemented, starting to collect data.

### Day 20: January 21, 2017

**Today's Progress**: Collecting data, refining style of modal and general layout.

### Day 21: January 22, 2017

**Today's Progress**: Completed data collection; interactive map now complete and
working. Need to consider mousewheel events in Firefox, do **not** work and looks
as though a fix is fiddly. Also need to add menu, lookup "near me" and then
investigate adSense/cookies.

### Day 22: January 23, 2017

** Today's Progress**: Finished writing a front (index) page and some
re-factoring of code for re-use. Need to write the search page ...

### Day 23: January 24, 2017

** Today's Progress**: Started work on search page for ukskislopes

### Day 24: January 25, 2017

** Today's Progress**: Converted serving of the slopes JSON data from a
Heroku app; this gets the data away from GitHub and will allow the search
to be carried out by making a Heroku call rather than in-app (which will)
mean less strain locally and less data being pulled down).

### Day 25: January 26, 2017

** Today's Progress**: Worked out how to protect an API key in test and production
environments, dealt with requesting lat/long coords given place name or postcode
using Google Maps API (some issues but now dealt with). Now need to use that info to
generate a shorter GeoJSON list of slopes.

### Day 26: January 27, 2017

** Today's Progress**: Completed back-end (using Cloud9 and deployed to Heroku) to
enable both 'full' and 'search/' end-points - the latter expects to receive a place
name or postcode and returns a JSON list of slopes within 50 miles together with
their distance.

Also set up a Raspberry Pi to act as a local server with a copy of the front-end
files in order to see how the site renders on a mobile/tablet (some issues to be
overcome, particularly with pinch-to-zoom on the map).

** Next Steps**:
* Write the front-end search (so that the site is functional)
* Consider styling generally
* Consider styling specifically for tablet/mobile device (now that I have a
    server to see them)
* Check and finesse, particularly zoom in Firefox (desktop) and on mobile/touch
    browsers

### Day 27: January 28, 2017

** Today's Progress**: Dealt with touch events on the map screen; map now pans
and zooms in reaction to touch events, and touching a slope 'dot' makes the modal
visible (this was surprisingly difficult).

Finished writing the search page, website if now functionally complete (albeit
with some styling and finessing required).

No longer queuing calls for JSON data - instead make an immediate call for the
map (which is locally stored and should be rendered effectively immediately) and
then trigger a call for the slopes JSON from Heroku; slower overall load time
but should be perceived as faster; could make an immediate call for the slopes
data but avoiding the unlikely issue if slopes is rendered before country (in
which case suspect that the slopes would not be visible).

** Next Steps**:
* Consider specific styling requirements for mobile devices **and particularly**
    small (and small landscape) screens - suspect will need to resize text as a
    minimum in these circumstances
* Put a copy of the site live (probably on domwakeling.com) and ask for feedback

### Day 28: January 29, 2017

** Today's Progress**: Implemented some tweaks to the site (zooming out should
now re-center the page, improved layout on mobile devices, tweaks to search
results) & set the site live at ski-slopes.uk

### Day 29: January 30, 2017

** Today's Progress**: Researching Google Search Console, SEO optimisation and
Google AdSense; tweaks to site for SEO and performance. Transferred WP install
from local (using RPi as server) to hosted.

### Day 30: January 31, 2017

** Today's Progress**: For something a little different, did some coding on the
BBC Micro:Bit using MicroPython.

### Day 31: February 1, 2017

** Today's Progress**: Some more MicroPython on a BBC Micro:Bit ... because
"why not?"

### Day 32: February 3, 2017

** Today's Progress**: Setting up another domain, local development environment
and deployment, syncing via Atom/Remote-Sync, setting up redirects using a ```.htaccess
``` file.
