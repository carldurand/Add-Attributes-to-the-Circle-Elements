Data Visualization with D3: Add Attributes to the Circle Elements
The last challenge created the circle elements for each point in the dataset, and appended them to the SVG canvas. But D3 needs more information about the position and size of each circle to display them correctly.

A circle in SVG has three main attributes. The cx and cy attributes are the coordinates. They tell D3 where to position the center of the shape on the SVG canvas. The radius (r attribute) gives the size of the circle.

Just like the rect y coordinate, the cy attribute for a circle is measured from the top of the SVG canvas, not from the bottom.

All three attributes can use a callback function to set their values dynamically. Remember that all methods chained after data(dataset) run once per item in dataset. The d parameter in the callback function refers to the current item in dataset, which is an array for each point. You use bracket notation, like d[0], to access the values in that array.


Add cx, cy, and r attributes to the circle elements. The cx value should be the first number in the array for each item in dataset. The cy value should be based off the second number in the array, but make sure to show the chart right-side-up and not inverted. The r value should be 5 for all circles.

Passed
Your code should have 10 circle elements.
Passed
The first circle element should have a cx value of 34, a cy value of 422, and an r value of 5.
Passed
The second circle element should have a cx value of 109, a cy value of 220, and an r value of 5.
Passed
The third circle element should have a cx value of 310, a cy value of 380, and an r value of 5.
Passed
The fourth circle element should have a cx value of 79, a cy value of 89, and an r value of 5.
Passed
The fifth circle element should have a cx value of 420, a cy value of 280, and an r value of 5.
Passed
The sixth circle element should have a cx value of 233, a cy value of 355, and an r value of 5.
Passed
The seventh circle element should have a cx value of 333, a cy value of 404, and an r value of 5.
Passed
The eighth circle element should have a cx value of 222, a cy value of 167, and an r value of 5.
Passed
The ninth circle element should have a cx value of 78, a cy value of 180, and an r value of 5.
Passed
The tenth circle element should have a cx value of 21, a cy value of 377, and an r value of 5.