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
