Coordinate Systems in ArcGis are always a headache and usually the reason of some errors or why our results do not look as they should.
Therefore it is very important to set up correctly our coordinate system and to make sure that all our data has the same coordinate system.

# Define a coordinate system

If our data does not have any coordinate system defined we can do it with the <b>Define Projection</b> command (1). We just need to introduce the feature or dataset and to choose the coordinate system (2) we want to define from a given list (3).

![Defining CS](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Coordinate%20Systems/Defining%20CS.JPG)

When we import a table with X and Y coordinates and we extract that X,Y data as points into our map (see ArcGis/Tutorial/Basics.md Adding new data), the software itself will offer the option to select the coordinate system of those X,Y points:

![Defining CS Tables](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Coordinate%20Systems/Defining%20CS%20Tables.JPG)

# Spatial data projection

It can happen that not all our data is in the same CS, for that we got the <b>Projection</b> command which allows us to project the spatial data from one coordinate system to another.

We just need to introduce the feature or dataset (1), the coordinate system that the data already has it will appear automatically (2), but we have to define the output CS, that is, the same CS of our project and the rest of our features (3). The command will give then us a list with the <i>Geographic Transformations</i> from one CS to the other (4)

![Projection](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Coordinate%20Systems/Project.JPG)

Other option is to go to the <i>Layer Properties</i> and in the Coordinate Systems tab (1) select Transformations (2) and there we convert the current CS into the desired one (3).

![Layer Properties Transformation](https://raw.githubusercontent.com/biometry/ArcGis/master/Images/Coordinate%20Systems/Data%20Frame%20Transformation.JPG)
