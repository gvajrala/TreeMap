# TreeMap


![image](https://user-images.githubusercontent.com/100104323/159960858-7820211e-3475-40c4-9de4-a36fc386e845.png)

An interactive treemap chart for visualizing proportions in hierarchical data, where nodes of a tree are represented as nested fully-packed rectangular tiles.

Supports zooming interactions via mouse-wheel events or by clicking on a node, which focuses the viewport on the associated sub-tree. The chart also responds to data changes by animating the dimensions of each of the nodes into their new positions.

For improved performance, nodes with area (width*height) smaller than a given threshold (minBlockArea) are excluded from the DOM, allowing for representation of large data sets while maintaining a smooth interaction.
Quick start

