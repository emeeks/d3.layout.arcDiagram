# Arc Diagram

[Demo](http://bl.ocks.org/emeeks/8d75da95d1e78cd08899)

There's already [a much more complicated and feature-rich arc diagram layout for D3](http://bl.ocks.org/goodmami/fd03b250588e1e1143bd) available but I wanted to write a simple layout to demonstrate arc diagrams and for folks who wanted a simple arc diagram for whatever purpose.

**#arcDiagram.size** An array of [width, height] that is used to calculate the location of the nodes along a line (drawn at the height value) as well as the arcs (drawn using a basis-interpolated line with variable height depending on which nodes are connected).

**#arcDiagram.nodes** An array of the nodes of your network.

**#arcDiagram.links** An array of the edges of your network. As with other D3 network layouts, if the source and target properties are numbers, they are assumed to be array position within the nodes array, otherwise objects are assumed.

**#arcDiagram.arc** A drawing function that takes an edge datapoint and returns the drawing instructions for a path element.

