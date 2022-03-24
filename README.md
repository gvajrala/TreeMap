# TreeMap
An interactive treemap chart for visualizing proportions in hierarchical data, where nodes of a tree are represented as nested fully-packed rectangular tiles.

Supports zooming interactions via mouse-wheel events or by clicking on a node, which focuses the viewport on the associated sub-tree. The chart also responds to data changes by animating the dimensions of each of the nodes into their new positions.

For improved performance, nodes with area (width*height) smaller than a given threshold (minBlockArea) are excluded from the DOM, allowing for representation of large data sets while maintaining a smooth interaction.
Quick start

import Treemap from 'treemap-chart';

or

const Treemap = require('treemap-chart');

or even

<script src="//unpkg.com/treemap-chart"></script>

then

const myChart = Treemap();
myChart
  .data(<myData>)
  (<myDOMElement>);
  Data syntax

{
  name: "root",
  children: [
    {
      name: "leafA",
      value: 3
    },
    {
      name: "nodeB",
      children: [
        {
          name: "leafBA",
          value: 5
        },
        {
          name: "leafBB",
          value: 1
        }
      ]
    }
  ]
}
