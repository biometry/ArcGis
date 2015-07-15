# Creating the Area Fishnet

The first step will be to create a Fishnet given a specific area.

![Create a Fishnet](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Fishnet/Create%20Fishnet.JPG)

There are a couple of things to consider on the <i>Create Fishnet</i> command:

*1 <b>Template extent</b>: that will be the extension of our Fishnet, I selected the study area in this case (<i>areas2</>. This way the Fishnet coordinates will be filled automatically.

*2 <b>Cell Size Width/Height</b> & <b>Number of Rows/Columns</b>: Here we can choose to set up how many rows and columns we want or how big the cells from the fishnet will be. It is important to, at least, filled 2 of these options.
I, for example, wanted 13 rows and 19 columns, so I set up the cell sizes as 0, this way ArcGIS will calculate them automatically.

*3 <b>We can create a label of points, so a point will appear in the middle of each cell. I did not select this option this time.

*4 The last part will be to set the fishnet as a polygon or as a polyline. I prefer polygon.

![Create a Fishnet Command](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Fishnet/Create%20Fishnet%20Command.JPG)

# Intersecting the Fishnet with the Points

Our objective will be to show the amount of points, in this case, in each cell from the fishnet grid. For that, we will use the command <b>Analysis Tool->Overlay->Spatial Join</b>

![Spatial Join](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Fishnet/Spatial%20Join.JPG)

In <i>Target Features</i> we will have to set the fishnet layer, and the point data in the <i>Join Features</i>. We leave the rest of fields as per default.

In order to have a better visualization from the point frequency we will have to modify the symbology of the new join layer. In <b>Properties->Symbology</b> we select the <i>Chart</i> and <i>Bar/Column</i>, the field will be the new created <i>Join_Count</i>.
Setting up the background color as trasparent will help us to have a better overview.

![Symbology](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Fishnet/JoinCounts.JPG)

![Columns](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Fishnet/Columns.JPG)



