# Creating a Carpentries Intro slideshow

## Installation

Follow reveal-md installation steps here: https://github.com/webpro/reveal-md#installation

## Clone this repo to your computer

Either use the git command line tool to run:

```
git clone https://github.com/MikeTrizna/carpentries_intro_reveal
```

or use the GitHub Desktop app to File > Clone Repository, and then paste in this repo ULR.

## Make edits to intro.md

Edit intro.md to make sure info is up-to-date.

## Make slides

```
reveal-md intro.md --static intro
```

This command will create a static website in a new directory called "intro".

## Move slide website to course website

Copy the contents of the new directory "intro" directly into the top level of the workshop "gh-pages" branch. Check out the "intro" folder here: https://github.com/SmithsonianWorkshops/2020-05-19-smithsonian/tree/gh-pages

You can then add "/intro" to the end of the course website URL to get to the Intro slides web page. For example: https://smithsonianworkshops.github.io/2020-05-19-smithsonian/intro

## Print PDF

This step requires having puppeteer installed (https://developers.google.com/web/tools/puppeteer/get-started). 

```
reveal-md intro.md --print intro.pdf
```