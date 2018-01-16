Assignment 1 - Hello World: GitHub and d3  
===
I started this assignment by trying to think about something
I would like to see visualized that would incorporate many of the 
graphics primitives the assignment is designed to get students comfortable with.
I settled on the career paths of students in the CS industry. I figured this would
be interesting to many others in the class as well. To simplify, I essentially just 
made up a few different career trajectories as an example. Another interesting aspect
I would incorporate with more time would be a dropdown or search for a specific student
and a resulting linear path (a way to isolate a student from the group).

Technical Achievement
---
My technical achievement in this assignment is primarily going past just displaying graphics primitives, to using
graphics primitives in a more complex visualization. Additionally, I practiced reading in data from a json file, and working with
nested hierarchical data.

While I did start with an example from the d3 docs, working with hierarchical data still proved challenging
because I had to fit the code to my data. Understanding the way d3.hierarchy() function works in terms of generating 
children was valuable to learn. Something that looks relatively simple but was actually quite difficult was placing text inside the 
rectangle elements. It's actually not possible to append a text element to a rectangle in svg so I had to first place the rectangle
then place the text on top. With more time I would probably try to convert the rectangles with labels to a dropdown menu or some sort of 
collapsible structure bound to the array of students.

Design Achievement
---
My design achievement in this assignment consists of a structured approach to choosing
a visualization, reading in colors from a json file, as well as incorporating interactivity and animation.

I started this assignment by just thinking about how I would visualize
this phenomenon in my head. What resulted was a trie-type structure with heatmap
properties as well displaying commonly taken paths. I then turned to the D3 docs to evaluate 
what types of pre-existing visualizations might fit well. The initial options
I considered included: sunburst diagram, node-link tree, collapsible force layout, and collapsible
tree layout. I ended up choosing the collapsible tree layout because it matched most closely to what
I had initially visualized in my head and the other visualizations seemed to have extraneous features
I wouldn't be able to fully take advantage of in this assignment. Secondly, each rectangle in the collapsible tree diagram reads
its color from the json file that is initially read in to generate the structure. The colors are svg standard color strings. Lastly, the visualization
is interactive and animated. It's possible for the user to click on nodes and expand children, then close them back again. Transitions are visible as nodes expand
which increases the aesthetic appeal of the design, acting in a way that feels natural to users.

Sources
---
https://bl.ocks.org/mbostock/4339083
https://gist.github.com/davo/4186300
https://www.dashingd3js.com/svg-basic-shapes-and-d3js
http://www.december.com/html/spec/colorsvg.html
https://groups.google.com/forum/#!topic/d3-js/Jx1hG5v9ivI
https://github.com/d3/d3
https://bl.ocks.org/d3noob/43a860bc0024792f8803bba8ca0d5ecd
https://www.thinkful.com/learn/a-guide-to-using-github-pages/start/existing-project/project-page/existing-repo/