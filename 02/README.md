# 02

let's draw a different path on this map

do this to learn about drawing paths on maps

to trace the path I used this tool [http://geojson.io/#map=4/56.05/113.29](http://geojson.io/#map=4/56.05/113.29)

and this tool to convert geojson to topojson [http://jeffpaine.github.io/geojson-topojson/](http://jeffpaine.github.io/geojson-topojson/)

then I pasted the 
- `arcs` array
- `transform.scale` array
- `transform.translate` array

into the topojson file I'd adapted from `transsiberian.json`
 
---

Creating visualizations like [this one](http://bl.ocks.org/rveciana/8464690) but using canvas is possible.

The technique is [the same as when using it with SVG](http://stackoverflow.com/questions/25442709/draw-html5-javascript-canvas-path-in-time) with the problem that Canvas hasn't got a method to get the whole length of a path. To do it, I've created a hidden SVG first. [This other page](https://css-tricks.com/svg-line-animation-works/) has a nice explanation about how the SVG path animation work.

The path is the Trans Mongolian train route [taken from here](http://gisforthought.com/trans-siberian-on-github) but redrawn, since the original is a multi line.
