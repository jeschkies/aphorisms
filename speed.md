https://stackoverflow.com/questions/418914/why-is-c-so-fast-and-why-arent-other-languages-as-fast-or-faster?page=1&tab=votes#tab-top<Paste>

This answer is probably going to land in the void but maybe it'll spark some ideas for someone at some point. I've optimized concurrent distributed system, improved the speed of Machine Learning code and dug into rendering code to see what's makes it fast.

# Type of Speeds #

## Development Speed ##

Before I'll talk about C let's look at what we mean when we talk about speed. I assum that the question is not about speed of development iterations. This is where Python and Ruby (or rather Ruby on Rails) or Elixir often prevail. For Machine Learning this can also be Julia or Python with Jupyter notebooks.

## I/O Bound ##

When we talk about speed we often talk about benchmarks and which implementation in which language gets the highest score. I'll distinguish between benchmarks for *I/O* bound tasks and for *compuation* bound tasks. Let's look at I/O bound tasks. There we have to distinguish between number of I/O operations and data transfer speed. An example for the former is a web server that receives clicks on a website such as Amazon or Facebook. 

## Computation Bound ##
