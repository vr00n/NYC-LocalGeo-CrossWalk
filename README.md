# NYC-LocalGeo-CrossWalk
*This is something that I've been meaning to do for a very long time. Hope it serves well.*

A single relationship file that links up all the local geographies in New York City.

[Link to Carto Map with same data](https://nyu.carto.com/u/varun-cusp2/builder/8ba55666-2289-4206-8165-60fc4601e35c/embed)

[Link to Google Sheets](https://docs.google.com/spreadsheets/d/e/2PACX-1vS1YkNk0JlVNrJehoDvbyodd0zkqyh19MkRmqaYV6CRyDLFwquuv0VbJ9iY2UeormzFZZ3Z0k6dkUmO/pubhtml#)

**What is this?**

A single csv file that *walks* across all of New York City's local geographies. This file links up the following geographies in a single tabulated file:

 - Borough Boundaries 
 - Census Blocks 2010 
 - Census Tracts 2010 
 - City Council Districts 
 - Community Districts 
 - Election Districts 
 - Fire Battalions 
 - Fire Companies 
 - Fire Divisions 
 - Health Area 
 - Health Center 
 - Municipal Court Districts 
 - Neighborhood Tabulation Areas
 - Police Precincts 
 - PUMA
 - School Districts 
 - State Assembly Districts 
 - State Senate Districts 
 - U.S. Congressional Districts 

**Why do we need this?**

This dataset could help answer questions like this more easily while also reducing the overall friction to integrate data from disparate domains.Example:

    In New York City:
	    How many and which Census Tracts are located in School District 31?
	    AND 
	    Which Fire District is serviced by this School District?
	    AND 
	    Which City Council District is this School District in?
	    AND 
	    Which Congressional District is it in?
	    AND
	    How many Health Centers are in this area?
	  


**How was this done?**

I combined all the shapefiles from NYC.gov's [Political and Administrative Districts - Download and Metadata](https://www1.nyc.gov/site/planning/data-maps/open-data/districts-download-metadata.page) using QGIS's "Join attributes by location" and performing an Interesection operation. The result was an attribute table that work as a relationship file to connect all the intersecting geographies.


Here is a similar crosswalk visualized for US Census Data:

![enter image description here](http://mcdc.missouri.edu/geography/sumlevs/censusgeochart.png)
