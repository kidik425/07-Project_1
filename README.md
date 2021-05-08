# 07-Project_1
# Team Name: Eff {Strings}

### - "A LastFM data exploration project." -

### __Members:__ Amber, Christian, Ishmael, Steve



__Repo Owner:__ Steve


__Repo Directory__

* Input folder - contains csvs for the analysis
* LastFM folder - contains jupyter notes for the overall project and a sub folder containing the individual contributions
* Ouput folder - contains pngs of the graphs used for analysis
* Team Organization Documents folder - used for the team for documentating our thoughts and process

__Branches (Owner: Name)__



* Amber: Amber_Top_Artists_Hungary - personal analysis notebook
* Steve: Steve Analysis - personal analysis notebook
* Christian: Christian_analysis - personal analysis notebook
* Group

    : LastFM_Analysis - consolidated analysis notebook
    
    : LastFM_Dataset_Pull_Cleanup - datapull and cleanup notebook

__Why LastFM????__
As a team we wanted to stick with data related to topic we enjoy.  First we wanted to go with something food related and found that the one source we were hoping to use no longer offered API support.  We went back to the drawing board of choosing.  After a few minutes of brainstorming, we quickly thought... MUSIC!!!!!

This lead us to look into the data offered by different platforms like Spotify, Music Story, and Apple. After some exploring of what the different platforms offered in terms of ease to use and data we ended up finding LastFM. 



__Questions:__

* Q1 Who are some of the popular artists across different countries?
* Q2 What are some of the popular genres?
* Q3 Is there a similarity to the artist across different countries?
* Q4 Hypothesis - Due to the popularity of giant streaming sites like Spotify, Pandora and Apple, we assume that LastFM isn't as popular as those.  That said, if a country's GDP is low then LastFM listenership is higher.



__Tools Used:__

* LastFM API
* .csv files
* Python (using pandas, matplotlib and other various dependencies)
* Jupyter and VS Code for coding
* Powerpoint for the presentation
* Zoom for communicating/meeting
* Slack for more communicating



__Notebook Usage:__

Any branch with a person's name on it is used by that individual to do their own research and analysis against the data.

The notebook with "LastFM" is used for the overall project deliverables.



__Data ETL Approach:__

Api calls against the LastFM data agents. Started by getting a list of countries from an ISO1866 pull (LastFM supposedly uses these names as in the data collections).  Once the countries are stored in csv, we then loop through each of those countries pulling the top 50 artists played on LastFM.  This information was also stored as a csv.

Some countries were missed, and we did a manual clean up of those names by looking for countries that had 0 counts of artists.  In the country.csv we corrected some in order to get that information from LastFM.

Then, took that csv of top artists and pulled their playcount, genre and listenership from LastFM.

We ended up cleaning this data by looking at the list of genres and grouping them into a subset of super genres.

Lastly we grabbed a GDP csv from the World Population Review website.  We also retrieved Lat and Long; Lat and Long were for a GMAP chart that did not make it into the project. 

 


__Data Analysis Approach:__

After getting the data we wanted, we divided analysis effort of the data sets to come up with the graphs in each person's individual notebook.

 

__Outcome__

We found that our Hypothesis did not correlate and that the GDP of country is not a determing factor in the listenership of LastFM.