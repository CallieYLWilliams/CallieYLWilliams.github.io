# CallieYLWilliams.github.io
Plant Database

## Add New Plants

Download code from https://github.com/CallieYLWilliams/CallieYLWilliams.github.io (Via git clone or otherwise) e.g.

	git clone https://github.com/CallieYLWilliams/CallieYLWilliams.github.io.git
	
Add images with appropriate names to /img folder e.g.

	Birchtree.jpg
	
Edit PlantDatabase.csv located in /data folder, and add the information for the new plant using the strucutre defined as

	Name,Latin Name,Appearance,Light Microscope Image,Light Microscope Description,Scanning Electron Microscope Image
	
e.g.

	Shepherd's Purse,Capsella bursa-pastoris,img/ShepherdPurse.jpg,img/ShepherdPurseLM.jpg,,img/ShepherdPurseSEM.jpg
	
Once all new plants are added, changes need to be pushed to git:

1. `cd D:\Shortcuts\Documents\Callie\Website\CallieYLWilliams.github.io` - Change to working directory in terminal
	
2. `git add --all`	- (adds all changed and new files to the repositry)
	
3. `git commit -m "NAME_OF_COMMIT"` -('saves' changes locally)
	
4. `git push -u origin main` - (pushes changes to the github repositry ('internet') so it can be publically accesed and viewed on https://callieylwilliams.github.io/)
	
	
## Technical Details

- /css - Style sheet for whole website
- /data - PlantDatabase.csv belongs here
- /img - Images of plants referenced in PlantDatabase.csv are stored here
- /js - Javascript file for transforming .csv to html for webpage
- index.html - landing page for website where all database is displayed

index.html

- Sets up format of page to show title and background image as well as defining the location for the database table
- Script section activates when page first opens and triggers the creation of the table from the PlantDatabase.csv

csv_to_html_table.js

- When called, this function will read the PlantDatabase.csv and convert to a HTML table to displayed
- source: `https://github.com/derekeder/csv-to-html-table`