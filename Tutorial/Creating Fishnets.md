# Creating the Area Fishnet

The first step will be to create a Fishnet given a specific area.

![Create a Fishnet](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/ArCatalog/ArcCatalog-Connecting%20directory.png)

There are a couple of things to consider on the <i>Create Fishnet</i> command:

*1 <b>Template extent</b>: that will be the extension of our Fishnet, I selected the study area in this case (<i>areas2</>. This way the Fishnet coordinates will be filled automatically.

*2 <b>Cell Size Width/Height</b> & <b>Number of Rows/Columns</b>: Here we can choose to set up how many rows and columns we want or how big the cells from the fishnet will be. It is important to, at least, filled 2 of these options.
I, for example, wanted 13 rows and 19 columns, so I set up the cell sizes as 0, this way ArcGIS will calculate them automatically.

*3 <b>We can create a label of points, so a point will appear in the middle of each cell. I did not select this option this time.

*4 The last part will be to set the fishnet as a polygon or as a polyline. I prefer polygon.

![Create a Fishnet Command](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/ArCatalog/ArcCatalog-Connecting%20directory.png)
