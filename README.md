### Overview:

New Yorkers can call into the 311 hotline to access non-emergency city services.  These calls cover a wide variety of topics; from items lost in taxis to support to assistance for elderly facing evictions.  Information on the calls that New Yorkers make to 311 is available for our analysis via NYC OpenData.  We analyzed this dataset to determine what the changing nature and volume of these calls indicates about a neighborhood.

### Data Source:

NYC 311 calls from 2010 to present.  Accessed via NYC OpenData API.

311 calls subsetted to the below departments:

* 	HPD (Housing Preservation and Development)<br/>
* 	NYPD (Police Department)<br/>
* 	DSNY (Department of Santiation)<br/>
* 	DOT (Department of Transportation)<br/>
* 	DOB (Department of Buildings)<br/>
* 	DPR (Parks and Recreation)<br/>
* 	DHS (Homeless Services)<br/>
* 	DFTA (Department for the Aging)<br/>
* 	DEP (Environmental Protection)<br/>

### Process:
1.	Using the OpenData API we pulled in data for nine departments that had both a high volume of calls and would give us an indication of the changing nature of a neighborhood.  

2.	We cleaned up our data by re-calculating the community board into a format that worked with our Bokeh shapefile, removing rows that did not have community board location, and creating dummy columns for the different complaint types within each department.

3.	Next, we aggregated our data into monthly totals by community board, by department.

4.	Finally, we mapped our data onto our Bokeh map to show how the number and types of complaints changes over time.

### Map Sample Images (download notebook and run to use slider):

!![Image of Yaktocat](https://github.com/PDibert/nyc_open_data_hackathon/blob/master/images/bokeh_plot.png)
![GitHub Logo](/images/bokeh_plot.png
