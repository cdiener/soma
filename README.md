soma
====

A small (<2kb) opiniated CSS framework using material design principles and some twists.

Soma stands for Small Opiniated MAterial design and gives you a tiny CSS framework based on [mincss](http://mincss.com) with some additional functionalities and a look and feel oriented on the principles of material design. This is not a fork of min.css since it changes some parts and adds new functionalities and is as such not compatible with min.css. If you want a fork which only converts the min.css design to material design look you can check out [my fork](http://github.com/cdiener/min).

## How do is use it?

For now there is no great documentation concerning usage, however, there is a demo page (index.html) showcasing
all the features. 

## How small is it?

Minified and gzipped soma.css is less than 1.6kB making it a fast loading alternative to heavier CSS frameworks.

## What does it include?

Soma includes the following components:

component       |  size (min+gzip) 
----------------|-----------------
general styles  |
responsive grid |
navbar          |
buttons         |
code blocks     |
headings        |
tables          |
timeline        |

Of course, you can customize which components you really want. In the less and scss directories there is an 
"all" file which allows you to only include the components you need.

## How to build?

If you want to build your own, the less and scss directories include a small build script wrapping the CSS
preprocessors. 
In order to build the less version you will need [less](http://lesscss.org/) installed with the [clean css plugin](https://www.npmjs.com/package/less-plugin-clean-css).
In order to build the scss version you will need [SASS](http://sass-lang.com/) installed.
 
