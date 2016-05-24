soma
====

A small (<2kb) opiniated CSS framework using material design principles and some twists.

Soma stands for Small Opiniated MAterial design and gives you a tiny CSS framework based on [mincss](http://mincss.com) with some additional functionalities and a look and feel oriented on the principles of material design. This is not a fork of min.css since it changes some parts and adds new functionalities and is as such not compatible with min.css. If you want a fork which only converts the min.css design to material design look you can check out [my fork](http://github.com/cdiener/min).

## How does it differ from other frameworks?

As the name suggest soma is opiniated by what I thought would be some nice assets for a CSS
framework. I think there is a set of minimal components we can all agree on such as a responsive
grid system, navbars and maybe buttons. However, I also included some components I found to be
useful various times such as some basic styling for source code blocks, social badges and formatting
for time-based data such as CVs. On top of it I tried to find some minimal styling which would be
compatible with the Material Design metaphor.

## How do is use it?

There is still no great documentation concerning usage, however, there is a demo page (index.html) showcasing
all the features. You can check out the source in order to see how to use the framework or see
the examples in the documentation :)

## How small is it?

Minified and gzipped soma.css is less than 2kB making it a fast loading alternative to heavier CSS frameworks.
To be exact `stat -c%s soma.css.gz` currently clocks in at 1750 bytes.

## What does it include?

Soma includes the following components:

File		| size (min + gzip)
----------------|-------------------
all	| 1750
buttons	| 360
cards	| 259
code	| 169
colors	| 36
forms	| 259
general	| 293
grid	| 200
headings	| 122
navbar	| 444
tables	| 120
timeline	| 631

The byte values add up to something slightly larger than the entire framework because the individual
components always need to include the color definitions contained in `colors.*`.

Of course, you can customize which components you really want. In the less and sass directories there is an
"all" file which allows you to only include the components you need. However, you will always need to include
`colors.*` to prevent compile errors.

## How to build?

If you want to build your own, the less and sass directories include a small build script wrapping the CSS
preprocessors.
In order to build the less version you will need [less](http://lesscss.org/) installed with the [clean css plugin](https://www.npmjs.com/package/less-plugin-clean-css).
In order to build the sass version you will need [`sassc`](https://github.com/sass/sassc) installed.
