# Marc to UF Digital Collections
Here lists steps and OpenRefine json codes needed to convert MARC .dat files to csv files that can be ingested into UF Digital Collections. 

![image](https://user-images.githubusercontent.com/13337446/215325755-4a419535-9192-4b92-b0bf-a05e4945421f.png)

1. Organize the data set in spreadsheet. OCLC number of Electronic Records are required.
2. Search, group and export records. 
Pull out the records via OCLC Connexion ID search
Save the whole batch in Local Save File (To save, use F4). (Please make sure Local Save File has been cleaned before starting a new batch.)
Search Local Save File (To open the search box: F3) --> OK --> Choose all files saved in  Local Save File and Export (F5) them as .dat file
3. Locate and rename the .dat file using the date and keywords from the project/batch (one filenaming method). .dat files are usually saved at the selected location when setting up OCLC on the work station. 
4. Convert  dat.file to txt files

Tools --> Export --> Export Tab Delimited Records

Set File Paths
Set the path for the dat.file: click the first file folder icon to locate and select the dat.file prepared during Step 2 and 3
Set the path for the exported txt file: click the second file folder icon to browse to the folder where the txt should be saved and name the txt file with the same name of the dat. file
Set In field delimiter to " | " 
Load the mapping document
--> Next --> Settings...--> Load Setting --> choose the map file (latest version: tobeudpated)
--> Export --> a pop up window will immediately notify the txt file has been created.
In OpenRefine

5. Create the new project in OpenRefine

Locate OpenRefine folder and Click the blue diamond to load OpenRefine in the browser as a new tab
In the browser OpenRefine tab, create the project
Get data from This Computer --> Choose File --> browse to locate the txt file prepared in Step 4--> Next
Parse data as CSV / TSV / separator-based files --> Character encoding --> UTF-8 --> check Trim leading & trailing whitespace from strings --> Create Project
