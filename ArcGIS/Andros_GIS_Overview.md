# Getting started with ArcGIS Pro:

__GIS:__ (Geographic Information System) An integrated collection of computer software and data used to view and manage information about geographic places, analyze spatial relationships, and model spatial processes. (from [*A to Z GIS*](https://search-library.ucsd.edu/permalink/01UCS_SDI/ld412s/alma991001005319706535))

__Visit:__
- [GIS Library guide](https://lib.ucsd.edu/gis)
- [Data & GIS Lab](https://lib.ucsd.edu/data-gis-lab)


__Documentation:__
- Esri's help docs are excellent and are available here: [ArcGIS Pro help](https://pro.arcgis.com/en/pro-app/help/main/welcome-to-the-arcgis-pro-app-help.htm)

### Starting a project  

1. Open up Pro and sign in. (use your full email address)
    ![Signing in][ARCPRO99]  

2. Create a new project (select Map)  

    ![Setting up your project][ARCPRO1]  

3. Name your project and tell Pro where to save it. *Note:* If you already have created a folder for your project, you can unclick the Create new folder option.  

    ![Name your project][ARCPRO2]

    __Connect a GeoDataBase__

4. From the Insert tab add data folders or connect geodatabases where your data lives:  

    ![Connect your folders][ARCPRO3]

    __Add a map__

5. From the Insert tab, click New Map to add a map:  

    ![Insert a map][ARCPRO4]

### The ArcGIS Pro Desktop Interface:
![The ArcGIS interface][ARCPRO5]  

> **Contents pane**
> 
> The left pane in ArcGIS Pro is called the Contents pane.  When a map 
> view is active, the **Contents** pane lists all the map layers found in the 
> map window and shows what the geographic features in each map layer 
> represent (points, lines, polygons, images, tables).  The **Contents** pane 
> helps you manage the display order of map layers and symbols used to represent 
> layers, as well as set the display and other properties (e.g. color, 
> line thickness) for each map layer.  It is also the place where you can 
> easily see the drive paths where your files are physically located on the 
> computer (e.g., C:\\temp\\mygisfiles).
> **It is very important to remember where your files are located when you are 
> working on a GIS project. In a GIS environment you will be doing a lot of data
> processing which requires the creation of new files, which must be
> saved. If you don’t know where you saved a file, your instructor is
> not going to know either.**
> When another view is active, such as the catalog view, the **Contents**
> pane will change to display the elements related to that view. 

>At the top of the **Contents** pane is a toolbar that controls how the layers are listed, and >what you can do to them. You can hover over the buttons to see tooltips for their function:

>  - List By Drawing Order
>  - List By Data Source
>  - List By Selection
>  - List By Editing
>  - List By Snapping
>  - List By Labelling

__Interface Tips:__
- The interface should look vaguely familiar--it is essentially a copy of Microsoft Office!
- Tabs across the top are dynamic; some only appear when needed.
- You may use the Map tab most often, but you'll also use Analysis and Insert a lot.
- Note the tabs across the far right of the Window. You'll often find useful tools like the Catalog and Toolbox menu here, and these can be pinned for quick access.


# Compatible Data Types & Formats:

### Supported Vector Data types:
- [Shapefile (.shp)](https://en.wikipedia.org/wiki/Shapefile)
- [GeoDataBase (.gdb)](https://desktop.arcgis.com/en/arcmap/10.3/manage-data/administer-file-gdbs/file-geodatabases.htm)  

<img src="https://upload.wikimedia.org/wikipedia/commons/3/38/Simple_vector_map.svg">  
Vector data example

[(wikimedia)](https://upload.wikimedia.org/wikipedia/commons/3/38/Simple_vector_map.svg)

### Supported Raster Data types:
- [GeoTIFF](https://en.wikipedia.org/wiki/GeoTIFF)
- [JPEG](https://en.wikipedia.org/wiki/JPEG)
- [ASCII](https://en.wikipedia.org/wiki/ASCII) (nightmare)
- [More!](https://gdal.org/drivers/raster/index.html)

<img src="https://docs.qgis.org/testing/en/_images/raster_data_zoomed.png" alt="Raster image">  
Raster data example


### Adding Data  

1. The standard way to add data is pressing the Add Data button on the Map tab:  
    ![Add data button][ARCPRO6]  

2. You can also drag and drop from the Catalog Tab:
    ![Add data from Catalog][ARCPRO7]

    As you add data to your Table of Contents, your drawing order matters. Those layers on top will be most visible. You can rearrange the order of items.

    ![Drawing order][FIG2] 

### Data Properties and Attributes  

1. Right click on a layer in the Table of Contents to view Properties.  
2. You can also right click to view the Attribute Table:  

    ![Right click on a layer][ARCPRO8]  

- Familiarize yourself with the data layer's properties and attribute table... *they are important!*  


## GIS and the Relational Data Model

An attribute table in ArcGIS is composed of **records** (rows) and **fields** (columns):

![Attribute table fields and records][FIG1] 

Right-click on each file in the **Contents** pane. You will see that you have different menu options for tables versus spatial data layers.

### Understanding How Tables Are Organized

1.  In the **Contents** pane, right-click on a vector layer
2.  Select **Open**.

3.  At the bottom of the table highlights how many records are hightlights out of a total number of records.   
    ![Records selected vs. total records][FIG3]

Right-click on a field name. What do you see?

The options you see are tools you can use to manipulate the data
contained in the field you’ve selected in various ways. For now, explore
the two sorting tools on your own; they’re self-explanatory. Below,
you’ll learn how the **Calculate Field**, **Calculate Geometry** and **Summarize** tools work.

Close the table.

[ARCPRO99]: img/UCSDOnline-LoginProcess.png "SignIn"
[ARCPRO0]: img/esrilogo.png "Esri logo"
[ARCPRO1]: img/ArcGIS1.jpg "start screen"
[ARCPRO2]: img/ArcGIS2.jpg "Name & save  your project"
[ARCPRO3]: img/ArcGIS3.jpg "Connect to folders or geodatabases"
[ARCPRO4]: img/ArcGIS4.jpg "Insert a map"
[ARCPRO5]: img/ArcGIS5.jpg "map interface"

[ARCPRO0]: img/esrilogo.png "Esri logo"
[ARCPRO1]: img/ArcGIS1.jpg "start screen"
[ARCPRO2]: img/ArcGIS2.jpg "Name & save  your project"
[ARCPRO3]: img/ArcGIS3.jpg "Connect to folders or geodatabases"
[ARCPRO4]: img/ArcGIS4.jpg "Insert a map"
[ARCPRO5]: img/ArcGIS5.jpg "map interface"
[ARCPRO6]: img/ArcGIS6.jpg "add data button"
[ARCPRO7]: img/ArcGIS7.jpg "add from catalog"
[ARCPRO8]: img/ArcGIS8.jpg "right click on a layer"
[ARCPRO9]: img/ArcGIS9.jpg "the attribute table"

[FIG1]: img/lab4_fig1.png "Attribute table fields and records"
[FIG2]: img/lab4_fig2.png "Drawing order"
[FIG3]: img/lab4_fig3.png "Records selected vs. total records"