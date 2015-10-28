# INFM600
The dataset is created for the INFM600- Information Organization Assignment

-------
Version
-------

Version 1.0 (October 2015)

-----
Files
-----

	* Libraries.xlsx
	* Elementary_School_Districts.xlsx
 	* Schools_Private.xlsx
 	* Libraries - Elementary Schools.xlsx
 
<h1> Datasets </h1> 
-------------------------------------------------
<em> Focal Dataset </em> - Howard County Libraries
--------------------------------------------------

	The focal dataset links the locations of the different libraries in the Howard County. It contains
	the name of the libraries, their ID, address and the geometric points. By visualizing and analyzing 
	this dataset, we can assess the area in the vicinity of the library to identify
	different primary schools. 
	
<i>	* R, Slivinsky (2015, April 28). Howard County Libraries. Retrieved October 27, 2015, 
	from https://opendata.howardcountymd.gov/Maps-Locations-and-Boundaries/Howard-County-Libraries/r2ng-89j6 </i>

----------------------------
<em> Secondary Datasets </em>
-----------------------------

	1) Elementary_School_District 
	
	This dataset talks about the locations of various elementary schools in the Howard County Region. It 
	contains the ID and name of the schools, the address and the geometric location.
	
<i>	* Howard County Interactive Map:  Schools - Elementary.
	Retrieved from: https://data.howardcountymd.gov/InteractiveMapV3.html?Workspace=IndividualLayer&Layer
	=general:Schools_Elementary&LayerName=Schools%20-%20Elementary#tab10. Date accessed: 10/27/2015 </i>
	
	2) Schools_Private

	This dataset shows about the locations of various private schools in the Howard County Region. It
	contains the ID and name of the schools, the address and the geometric location
	
<i>	* Howard County Interactive Map:  Schools - Private.
	Retrieved from: https://data.howardcountymd.gov/InteractiveMapV3.html?Workspace=IndividualLayer&Layer
	=general:Schools_Private&LayerName=Schools%20-%20Private#tab10. Date accessed: 10/27/2015 </i>

-------------------------------------------------------
<em> New Dataset </em> - Libraries - Elementary Schools
-------------------------------------------------------

	This dataset combines the focal dataset with Elementart_School_District dataset. 
	
	<em> The procedure used to combine the datasets are: </em>
	
	1.The Elementary_School_District dataset is linked to the focal dataset primarily using the Street2 field.
	This field consists of the city, state and zip code data which is  split as city and zip code in the focal
	dataset as separate columns  ( ignoring the state data) 
	
	2.The Steps involved in splitting Street2 column:
			•Highlight the Street2 column.
			•On the Data tab, click the Text to Column option.
			•In the Convert Text to Column Wizard, select Delimited option.
			•Select ‘Spaces’ in the options shown next.
			•Click the finish button. 
			
	3.The FID of the schools, geometric points of the Elementary_School_District dataset are placed under the 
	column FID and geom in the focal dataset respectively.
	
	4.The ES_Home column from the Elementary_School_District dataset has been added as an additional column to 
	the focal dataset.
	
	5.The modified version of the focal dataset is saved as a new dataset named as “ Libraries-Elementary Schools” 


	
	
	
------- 
License
-------

