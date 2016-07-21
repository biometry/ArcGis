# Error selecting features

A layer can be damaged and therefore, ArcGIS will not allow us to select any part of the feature neither with the <b>editor arrow</b> nor with the <b>select feature</b> command.

To fix it we will have to run a <b>Repair Geometry</b>

![Reapir Geometry](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Error/Repair%20Geometry.PNG)


#Error 001143

Happened during <b> Raster Calculator </b>
Solution: disable background processes in ArcGIS via the Geoprocessing Options dialog box.

#Error building a Raster Atributte Table

If the raster is single band, then we have to convert the raster values into a integer.

Say that we have a raster type float, and we determine that the data values are only necessary up to 4 decimal points, we can use the Raster Calculator to do:

Int(raster * 10000)
