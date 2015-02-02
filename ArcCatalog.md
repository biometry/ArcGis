ArcCatalog is an ArcGIS application useful to manage our project data:

  -Create new shapefiles, layers, tables, rasters, etc
  
  -Modify properties from our data (e.g. defining proyections)
  
  -Edit tables

# Connecting ArcCatalog to our proyect's folder

The firts thing to do when we start a new proyect is to organise well our data. As soon as the project starts to grow, so it will the number of shapefiles, rasters, etc and it will be complicated to find the files we want.

By clicking on <i>File->Connect To Folder</i> we can select the folder(s) that will appear on our <i>Catalog Tree</i> and work on them.

![ArcCatalog Connection](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/ArCatalog/ArcCatalog-Connecting%20directory.png)

## Data visualization

We can visualizate any file on the right side from the Catalog Tree when we click on it.

There are 3 options given to see the information related to the file:

  -Contents: merely quick info about the data
  
  -Preview: here we can choose between <i>Geograpy</i> preview or <i>Table</i> preview. It is possible to work on the <i>Attribute Table</i> here, though I prefer to do it directly on ArcMap

  -Description: metadata about the file. It is possible to be edited (e.g. description, thumbnail, scale)

![Data visualization](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/ArCatalog/data%20Visualization.JPG)

## Data creation

On <i>File->New-></i> we can create a new file (shapefile, layer, geodatabase, etc) that we can export later on to our project

![Data creation](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/ArCatalog/creating%20file.png)

In the following example we can see how to create a newshapefile. We just need to give it a name, a shapefile type (point, polyline, etc) and to define the coordinate system to make sure that is the same than our project.
In case we forget to define the coordinate system, it will be possible to define it on the shapefile already created as we will see later.

![Shapefile creation](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/ArCatalog/shapefile%20creation.JPG)

To add the new file to our proyect we can just drag it in 

## Data editing

Right click on the file allows us to manage them.

![ArcCatalog Editing](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/ArCatalog/Editing_Files.png)

Anyhow, we can also do the editing work directly on ArcMap
