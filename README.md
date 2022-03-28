# CallieYLWilliams.github.io
Plant Database

## Add New Plants

Download code from https://github.com/CallieYLWilliams/CallieYLWilliams.github.io (Via git clone or otherwise) e.g.

	`git clone https://github.com/CallieYLWilliams/CallieYLWilliams.github.io.git`
	
Add images with appropriate names to /img folder e.g.

	`Birchtree.jpg`
	
Edit PlantDatabase.csv located in /data folder, and add the information for the new plant using the strucutre defined as

	`Name,Latin Name,Appearance,Light Microscope Image,Light Microscope Description,Scanning Electron Microscope Image`
	
e.g.

	`Shepherd's Purse,Capsella bursa-pastoris,img/ShepherdPurse.jpg,img/ShepherdPurseLM.jpg,,img/ShepherdPurseSEM.jpg`
	
Once all new plants are added, changes need to be pushed to git:
	* 1. `cd D:\Shortcuts\Documents\Callie\Website\CallieYLWilliams.github.io` - Change to working directory in terminal
	* 2. `git add --all	- (adds all changed and new files to the repositry)
	* 3. `git commit -m "NAME_OF_COMMIT"` -('saves' changes locally)
	* 4. `git push -u origin main` - (pushes changes to the github repositry ('internet') so it can be publically accesed and viewed on https://callieylwilliams.github.io/)
	
	
## Technical Details


	