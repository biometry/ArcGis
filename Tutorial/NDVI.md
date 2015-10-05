* Download the Landsat 8 images from http://earthexplorer.usgs.gov/

* Load the Bands images in ArcGIS

![Landsat bands](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/NDVI/Landsat%20bands.PNG)

* We open the <b>Image Analysis window</b> from Windows-> Image Analysis and composite the Bands 2, 3, 4 and 5 (blue, green, red and near infrared)

!Band configuration](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/NDVI/Bands%20config.PNG)

* We will get as resoult a 3 band image, we can change the band order depending of what we want to explore.
In this case we want to calculate the NDVI. The combination will be:
** Red: band 4
** Green: band 3
** Blue: band 2

![Band combination](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/NDVI/Band%20combination.PNG)

The red areas represent the vegetation.

* Export the Composite 3 band into a TIFF file.

![Exporting the TIFF file](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/NDVI/export%20tiff.PNG)

* We create the NDVI layer in the <b>Image Analysis</b> window, but first  we have to set up the red and near infrared bands thus the definition of NDVI is the red band - the NIR band divided by the sum of both.
We will do that in <b>Options</b> in the <b>Image Analysis</b> window.

!Band configuration](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/NDVI/Bands%20config.PNG)

As we said, the red band is the number 3 and the NIR the 4.

Now we can finally calculate the NDVI.

![NDVI](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/NDVI/NDVI.PNG)

We can set up the colors for a better visualization of the NDVI.

![Result](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/NDVI/final.PNG)

* Attribute table: 
In order to get the attribute table of the TIFF data you can construct attribute table for raster dataset using Data Management Tools > Raster > Raster Properties > Build Raster Attribute Table in ArcGIS. In order to be able to construct such an attribute table, your raster should be of one band, statistics calculated, and of "integer type" (it could be 8-bit or 16-bit integer) 

You can save this float point raster as 8-bit integer using "Copy Raster" tool or you can classify your raster by Spatial Analyst Tools > Reclass > Reclassify option (you can define up to 256 class), and then work with this reclassified "thematic" layer. 

