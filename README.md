# Playfair

1. [What is Playfair?](https://github.com/equitablegrowth/Playfair#what-is-playfair)
2. [Features](https://github.com/equitablegrowth/Playfair#features)
3. [Tutorial](https://github.com/equitablegrowth/Playfair#tutorial)

## What is Playfair?

[You can try out Playfair online (loading, saving, and theming are all disabled). Click here.](http://www.austinclemens.com/Playfair/playfair.html)

Playfair is a web app for graphing data. It supports MANY different kinds of graphs, can be themed, and is intended to create ready-to-publish graphs with annotations. It was created to allow researchers at the Washington Center for Equitable Growth to assemble publication-ready graphs without having to rely on our (two person) design team. There are a lot of web graphing apps out there, but Equitable Growth has a fairly specific set of needs that required a unique solution. Playfair's major design priorities are:

1. [Power and flexibility (ggplot2-style graphing)](#power-and-flexibility-ggplot2-style-graphing)
2. [Annotation and on-chart editing](#annotation-and-on-chart-editing)
3. [Easy to deploy](#easy-to-deploy)
4. [Collaborative editing](#collaborative-editing)
5. [Easy to theme](#easy-to-theme)

#### What isn't Playfair?
Playfair isn't as easy to use as most graphing apps. In particular, Playfair requires long data instead of wide data and people who aren't accustomed to working with data often find this confusing. Combined with the large number of options Playfair has, this makes Playfair best for users with some data analysis experience.

## Features

### Power and flexibility (ggplot2-style graphing)
A lot of graphing apps will make you a barchart or a linechart. But EG's needs are sometimes more technical. Sometimes we need a dot plot of coefficients from a statistical model with lines indicating confidence intervals. Charting in Playfair is modeled after the ggplot2 package for R. Playfair is not nearly so powerful, but it uses the ggplot2 concept of overlaying various chart elements on top of one another to create a complex chart. Playfair does not care what type of data you have - dates, numbers, and categories are all understood. As you can see in the gif below, Playfair will also make a customizable key for you.

![alt text](http://www.austinclemens.com/Playfair/assets/ggplot2.gif "Adding geoms to a graph")

In addition, the layout of a Playfair graph is fairly flexible and can be edited using the settings tab. This makes it possible to create some chart types that are not specifically supported or that require significant alterations to Playfair's charting style. You might recognize the chart below, from Edward Tufte's The Visual Display of Quantitative Information. It is the canonical example of what people call slopegraphs or slope charts. The chart below was created in Playfair, admittedly with about 30 minutes of work. [You can compare it to the original here](http://charliepark.org/slopegraphs/).

![alt text](http://www.austinclemens.com/Playfair/assets/slopechart.png "Slope chart")

### Annotation and on-chart editing
Playfair includes a number of tools for adding annotations directly to a chart to help explain the graphic. These include adding arrows, callout lines, and arbitrary text annotations. On-chart editing refers to Playfair's tools for editing text, data, and other elements directly on the chart simply by dragging or right-clicking.

![alt text](http://www.austinclemens.com/Playfair/assets/annotate.gif "Annotating a graph")

### Easy to deploy
Playfair is super easy to deploy for even non-technical users. Clone this repository and open playfair.html. You've deployed playfair! If you want to use custom themes and save your graphs, you'll have to deploy Playfair to a server. This takes a little technical know-how but is basically as simple as uploading the Playfair folder to a server and changing the permissions for the scripts in the cgi-bin folder to 755.

### Collaborative Editing
Playfair allows you to save and load graphics you have made. There isn't much organization and there aren't permissions so this could get out of hand for a large organization but should meet the basic needs of small organizations.

![alt text](http://www.austinclemens.com/Playfair/assets/loading.gif "Loading a graph")

### Easy to theme
Playfair's current theme system is largely undocumented but parameters are clearly named and it should be relatively easy to create your own theme. Switching between themes is as easy as choosing the theme you want from a dropdown. This is the default theme:

![alt text](http://www.austinclemens.com/Playfair/assets/themeexample.png "The default theme")

## Tutorial

I've created a short tutorial that should help you figure out the basics of Playfair. Click here to view the tutorial.

1. [Loading data](http://www.austinclemens.com/Playfair/playfair_docs/tutorial1.html)
2. [A simple graph](http://www.austinclemens.com/Playfair/playfair_docs/tutorial2.html)
3. [Annotations](http://www.austinclemens.com/Playfair/playfair_docs/tutorial3.html)
4. [More complicated](http://www.austinclemens.com/Playfair/playfair_docs/tutorial4.html)
5. [The settings tab](http://www.austinclemens.com/Playfair/playfair_docs/tutorial5.html)

[You can try out Playfair online too (loading, saving, and theming are all disabled). Click here!](http://www.austinclemens.com/Playfair/playfair.html)
