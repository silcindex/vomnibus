                                  _ .--.
                                 ( `    )
                              .-'      `--,
                   _..----.. (             )`-.
                 .'_|` _|` _|(  .__,           )
                /_|  _|  _|  _(        (_,  .-'
               ;|  _|  _|  _|  '-'__,--'`--'
               | _|  _|  _|  _| |
           _   ||  _|  _|  _|  _|
         _( `--.\_|  _|  _|  _|/
      .-'       )--,|  _|  _|.` __      __                    _ _                   
     (__, (_      ) )_|  _| /   \ \    / /                   (_) |                  
    jgs`-.__.\ _,--'\|__|__/     \ \  / /___  _ __ ___  _ __  _| |__  _   _ ___  
                     ;____;       \ \/ // _ \| '_ ` _ \| '_ \| | '_ \| | | / __|
                      \YT/         \  /| (_) | | | | | | | | | | |_) | |_| \__ \
                       ||           \/  \___/|_| |_| |_|_| |_|_|_.__/ \__,_|___/
                      |""|      
                      '=='


Vomnibus is an assortment of handy data for making information graphics in Clojure and ClojureScript.
Add it to your Leiningen `project.clj`:

    [com.keminglabs/vomnibus "0.3.2"]

and check the instructions for [cljx](https://github.com/lynaghk/cljx) to configure compilation for [ClojureScript](https://github.com/clojure/clojurescript).

and just `:require` or `:use` whatever you need.

geo.us.states
-------------
`states`, map of state name to geoJSON shape, e.g.;

    {"Arizona" {:type "Feature", :id "04", :properties {:name "Arizona"}, :geometry {:type "Polygon", :coordinates [[[-109.042503 37.000263] [-109.04798 ...

geo.us.counties
---------------
`counties`, list of all counties in geoJSON shape.
*Note*, don't try running this one through Google Closure; it takes impossibly long to process.

geo.world
---------
`countries` map of country name to geoJSON shape


color-brewer
------------
Cynthia Brewer's color schemes by name, e.g.;

```clojure
(def OrRd-3 ["rgb(254,232,200)" "rgb(253,187,132)" "rgb(227,74,51)"])
```

For full list of colors, see [Colorbrewer](http://colorbrewer2.org/)


d3
--
`flare` and `flare-imports` data used in D3 & ProtoVis examples

d3-colors
---------
Categorical color schemes: `Categorical-10`, `Categorical-20`, `Categorical-20b`, `Categorical-20c`.


Licensing
=========

Colorbrewer
-----------
[Colorbrewer](http://colorbrewer2.org/) schemes under Apache 2.0.


United States state and county outlines
---------------------------------------
Taken from [D3.js](http://mbostock.github.com/d3), which is under MIT; Copyright (c) 2012, Michael Bostock, All rights reserved.
See [this commit](https://github.com/mbostock/d3/commit/254a8e3e78ff7cc448d3657c553218bdc90478c6) in D3 for methodology.


Changelog
=========

0.3.0 Incorporate CLJX; full ClojureScript support


&c.
===

What's with the name?
---------------------
"Omnibus" since it's an assortment of items.
The "V" is for "visualization".

Shouldn't the picture be a bus?
-------------------------------
Whatever, this hot air balloon looks rad.
Props to [Joan Stark](http://www.geocities.com/spunk1111/transp.htm).
