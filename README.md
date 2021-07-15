# byoc

Bring Your Own Code - a CODAP data plugin

## What is it?

The result of me hacking a {[learnr](https://rstudio.github.io/learnr/)} tutorial (a shiny_prerendered app) using one code exercise and more hacky Javascript I wrote to connect the output to CODAP.

This means if you want different packages to be available in BYOC, just change the `index.Rmd` for the {learnr} tutorial. 

I'm currently hosting BYOC on my personal shinyapps.io account, which is not for "public" consumption, just for a demo. Please copy this repo and publish your own app to try it out with your students etc.

To use the plugin with CODAP, just change the second part of the URL below to point to your public instance of BYOC :-)

`https://codap.concord.org/releases/latest/static/dg/en/cert/index.html?di=https://annafergusson.shinyapps.io/byoc/`

## How does it work?

To send a data frame to CODAP from R, use the function `update_table("tableName", dataframe)`. Um, what else? The current state of the code is stored each time you press the run button, so you can use the "Share" functionality of CODAP to set up code in advance and share with students etc. (or they can save their work).

That's it for now, but please get in touch if you have ideas or want to do something more with this. 

## Why did you make this?

My current research is focused on how to support learners (high school students & first stage university students) to move from GUI-driven tools (pointy, clicky, draggy etc.) to code-driven tools (text, formulae, syntax, etc.). Related to this, I'm interested in are "hybrid" GUI/code environments, and CODAP seemed to be good place to experiment with this approach. 

There's a lot going on for learners when learning "coding", so the idea behind the BYOC plugin was that perhaps the "code" focus could be on the articulation of the model and initially CODAP could be used for the visualisation of any data generated from the model. 

If you're interested, you can read more about my research here: Anna Fergusson & Maxine Pfannkuch (2021) Introducing teachers who use GUI-driven tools for the randomization test to code-driven tools, Mathematical Thinking and Learning, DOI: [10.1080/10986065.2021.1922856](https://doi.org/10.1080/10986065.2021.1922856)




