---
layout: page
plotting: true
title: MeshFcn
categories: optimization, benchmark, plotting
tags: plotting
fname: meshfcn
functionname: MeshFunction
---

Draws mesh of a function on the 3-dimensional space.

`meshfcn(FCN, X, Y)` draws the mesh of the function given by the 
handle `FCN` in the x-y plane defined over the intervals specified by `X`
and `Y`.

`meshfcn(FCN, X, Y, X_LABEL)` draws the mesh and uses `X_LABEL` as the 
label of x-axis.

`meshfcn(FCN, X, Y, X_LABEL, Y_LABEL)` draws the mesh and uses 
`X_LABEL` as the label of x-axis and `Y_LABEL` as the label of the y-axis.

`meshfcn(FCN, X, Y, X_LABEL, Y_LABEL, Z_LABEL)` draws the mesh and 
uses `X_LABEL` as the label of x-axis, `Y_LABEL` as the label of the y-axis 
and `Z_LABEL` as the label of the z-axis.

`meshfcn(FCN, X, Y, X_LABEL, Y_LABEL, Z_LABEL, PLT_TITLE)` draws the
mesh and uses PLT_TITLE as the title of the plot. 

`meshfcn(FCN, X, Y, X_LABEL, Y_LABEL, Z_LABEL, PLT_TITLE, USE_COLORBAR)`
if `USE_COLORBAR` is true, a color bar will also be drawn. 

`[H] = meshfcn(...)` returns a handle, `H`, to a  surface plot object. 
`AXIS`, `CAXIS`, `COLORMAP`, `HOLD`, `SHADING`, `HIDDEN` and `VIEW` set figure,
axes, and surface properties which affect the display of the mesh.

Example: 
{%highlight MATLAB%}
  x = -10:0.01:10;
  y = x; 
  meshfcn(@ackleyfcn, x, y, 'x_1', 'x_2', 'z', true)
{% endhighlight %}

See also: contourfcn, surffcn