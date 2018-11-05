# nlchp-mapping-project
Map of cities with active anti-panhandling statutes/ordinances for campaign by the National Law Center on Homelessness &amp; Poverty


## Hello and welcome!

### The Project:

The National Law Center on Homelessness & Poverty (https://www.nlchp.org/) is a national nonprofit legal group dedicated to preventing homelessness and poverty. This project was undertaken for a national campaign against anti-panhandling laws spearheaded by the NLCHP in coordination with a couple dozen other regional and national nonprofits. The map built here is meant to be a clear resource for press and policymakers to track the progress of the campaign. 
<br><br>
The most recent version of the map is available on the NLCHP's website at https://nlchp.org/images/panhandling_cities. 

### The Map 

![Map](https://github.com/mattymecks/nlchp-mapping-project/blob/master/SampleMapLabeled.png)
    


### The Juypter notebook

The code in the EDA notebook imports the data into a dataframe using pandas, explores the data a bit, cleans up a few issues with geo-coding, manipulates the data to make it easier to update, and persists the changes. The Mapping notebook handles preparing the data to be mapped and then mapping the cities onto a geoscatter plot utilizing Plotly. At the end of the notebook, you'll see two options for plotting. One plots in Juypter. This make it extremely easy to visualize the changes you're making as you make them. The other plots in html (and generates an html file). 
<br><br>
A quick note on some of the mapping code. I was having trouble getting a text box to appear correctly in the map, so I converted all of my colors from rgb ro rgba, which allows you to set the 'opacity' of a color. I then created a 'phantom' trace with only one completely transparent point on the map itself and added the 'subplot' text found in the "Note" section as the label for that trace so that it appeared nicely in line with the rest of the legend.  


### The CSVs

The city_info.csv data is a list of city/state pairs provided to the NLCHP by its partners and then given to me. I used the awesome service Geocodio (https://www.geocod.io/upload/) to get lat/lon coordinates for each city along with other information, which lives in the city_info_geocodio.csv file. Geocodio was free (for my level of usage) and was extremely easy to use (upload a csv, download a csv).


### The HTML 

The HTML was auto-generated by Plotly after I ran the Juypter notebook and is employed on the website to create the dynamic map. The HTML can be regenerated later. 


### About Me

At the time of this writing, I'm a recent graduate of the Data Science Immersive at the Flatiron School in NYC. I feel passionately about the power of better data to build better policy and a better world. Feel free to reach out to me on GitHub with questions about this project (@mattymecks) or you can find me on Medium (also @mattymecks) where I [wrote up this project.](https://towardsdatascience.com/make-your-data-science-projects-meaningful-a05a7bc7c14c) 


### License

Everything here is licensed under the Apache 2.0 license. 
