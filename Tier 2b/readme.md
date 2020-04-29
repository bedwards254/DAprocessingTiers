# Tier 2b - Full Processing without Restrictions
Tier 2b processing is done by staff, students, and interns as deemed appropriate. Tier 2b is built upon what was started with [Tier 2](https://github.com/bedwards254/DAprocessingTiers/tree/master/Tier%202). Tier 2b collections are those that contain relevant collection material, and do not have any restrictions put on them as determined in the Deed. These can be large or small, depending on the collection. Once the files are normalized and arranged, follow the Finding Aid Edits and Upload to Reading Room Server sections below and mark the collection as Tier 2b in the shelf list.

# Table of Contents
1. [Folder Structure Setup](#folder-structure-setup)
2. [Extraction](#extraction)</br>
•	[Pull down from Keep](#pull-down-from-keep)</br>
•	[FTK Imager](#ftk-imager)</br>
3. [Virus Scanning](#virus-scanning)
4. [Switching from BitCurator to Windows](#switching-to-bitcuratorubuntu-from-windows)
5. [XML Files](#xml-files)
6. [MD5 File Creation](#md5-file-creation)
7. [Deduplication](#deduplication)</br>
•	[FSLint](#fslint)</br>
8. [Normalizing Files](#normalizing-files)
9. Arranging Files
10. [TAR Files](#tar-files)
11. [Bagging Files](#bagging-files)
12. [Uploading to Keep](#uploading-to-keep)
13. Directory Listing
14. Finding Aid Edits
15. Upload to Reading Room Server

---

## Folder Structure Setup
1. Create a folder called [collectionName]_workingFiles
2. Inside of that folder, create 3 folders called: 
a. Original Disk Images;
b. Extracted Files; and
c. Working Files
3. In Original Disk Images, create folders for each disk image you’re pulling down from the Keep
4. Copy the folders you just made to Extracted Files

[Back to top](#table-of-contents)

---

## Extraction 
### Pull down from Keep
*Staff:* pull down images from Keep (just images, not any accompanying material) on Windows side </br>
**Note:** these will pull down with their PID as the identifying title, so be sure to pay attention to which one you are on to click and drag it to the proper folder in Original Disk Images </br>
**Note:** If a number is skipped in the Keep files, delete that folder from Original Disk Images and Extracted Files

### FTK Imager
*Student/Staff:*
**Using FTK Imager in Windows to extract the files**
1. Launch FTK Imager from the Desktop.
2. From the drop-down File menu, select “Add Evidence Item.”
3. Choose “Image File” and click “Next.”
4. Browse to image file in Original Disk Images and click “Finish.”
5. The selected image file will appear in the Evidence Tree Pane. Click the small + mark to the left of the image file. 
6. The next sub-folder down will note the file system in brackets alongside the virtual disk label. Right-click over this sub-folder and select “Export Files.”</br>
a. You’re looking for the [root] folder or the most granular folder you can find. 
•	Note: If all you see is “Unallocated space”, there was an issue with the image, and the folder number can be deleted from Extracted Files ONLY – keep the original disk image
7. Navigate to the Original Disk Images folder and the corresponding ID number for the image you have open, and hit “Enter”
8. Click “OK.”
9. Once the export has finished, a dialogue box will open with details of how many folders and files have been exported. Click “OK.”
10. Continue doing these one at a time, paying attention to what number you are on so it exports to the correct folder in Extracted Files

[Back to top](#table-of-contents)

---

## Virus Scanning
1. Once the files are extracted, select all of the folders in the Extracted Files folder (Ctrl+A)
2. Right click and select “Scan with McAfee Virus Defense”
3. A window will pop up showing how many files are being scanned
4. When done, it will say “Scan: Complete” and have a count of infected files below
5. If any files are infected, let the digital archivist know right away

Copy the files in Extracted Files to Working Files

[Back to top](#table-of-contents)

---

## Switching to BitCurator/Ubuntu from Windows
1. [Instructions here](https://bedwards254.github.io/testBDBC/jekyll/2019/01/22/BC-Windows-Switch.html) 
2. Eject the hard drive before doing this step, and turn off the hard drive dock OR disconnect the USB cable 
3. Shut down the computer fully when switching between the two

[Back to top](#table-of-contents)

---

## XML Files
1. In BitCurator, copy the XML files created in Tier 1 to the corresponding folder in Working Files</br>
a. Staff: locate the corresponding hard drive where the original disk images are stored</br>
i. See https://emory.box.com/s/ju2ekovp649mi5w0tbkcpegw8oxittbu for an updated list</br>
2. Before turning the hard drive dock, insert the hard drive with the original disk images into the LEFT slot on the dock
3. Turn on the hard drive dock and mount both hard drives in BitCurator (open file directory on right computer and click on each hard drive ONCE to mount them)
4. Locate “Copy2” on the desktop
5. Edit “Copy2” to match the correct file paths to copy all XML files from the collection on the original hard drive to the corresponding folders in Working Files on the new hard drive (unless working on the same hard drive, then even easier)</br>
**POST CODE HERE AND SHOW EDITS**</br>
*Note:* if a folder was deleted in the steps above because there was nothing in it or didn’t exist in the Keep, these will automatically skip in this process. </br>
6. Once copying is complete, eject both hard drives from the computer by clicking the arrow next to their names in the file directory and then right clicking and selecting “Safely Remove Drive”
7. Power off the hard drive dock and eject the left hard drive and put back in the cabinet. 
8. Turn back on the hard drive dock and re-mount the hard drive in BitCurator 

[Back to top](#table-of-contents)

---

## MD5 File Creation
*Create MD5 file for Working Files folder*
1. Select all the folders in Working Files
2. Right click and select “Scripts” and then “Calculate MD5 script”
3. A pop-up box will appear showing the progress
4. Once done, a file called md5 will appear in the main Working Files folder
5. Open it to check the contents

[Back to top](#table-of-contents)

---

## Deduplication
1. On the desktop, click the Forensics and Reporting folder
2. Double click FSLint to launch it

### FSLint
3. Once open, click the “+Add” button at the top left and navigate to the hard drive and Working Files folder. 
4. Double click the first folder in Working Files
5. Remove the “/” from the top box using the “X Remove” button under the “+Add” button
6. Make sure the tab on the left is set to “Duplicates”
7. Click the “Find” button on the bottom left of the screen to start finding duplicates within the one folder
8. In the results screen, right click and choose "within groups," then “select all but newest” then click “Delete” in the bottom right corner.
9. Click “Find” again to make sure everything else got deleted
10. On the left, choose the “Empty Directories” tab and click “Find”
11. Delete all the empty directories which appear
12. Do the same for the “Temp Files” tab
13. Repeat this process for other folders in the collection, removing and adding each one every time
14. Once done with the individual folders, add the Working Files folder as a whole and run the “Duplicates,” “Empty Directories,” and “Temp Files” options against everything at once

[Back to top](#table-of-contents)

---

## Normalizing Files
*[Switch back to Windows](https://bedwards254.github.io/testBDBC/jekyll/2019/01/22/BC-Windows-Switch.html) to normalize the files using Adobe PDF/Paint/GIMP/Excel/Word*
1. For Word and Excel files, select multiple (around 10) files at once, right click and select “Convert to Adobe PDF”
2. Navigate to the correct folder it should go in and hit “Save” in the first dialogue box; do the same for the second dialogue box. 
3. For TIFF/BMP/PNG files, right click and choose “Open With...” and choose Paint. Do these one at a time. In Paint, choose “Save As…” and choose JPG. Navigate to the proper folder and hit “Save”
4. For Photoshop/Illustrator files, right click and choose “Open With...” and choose GIMP. Click “Ok” when GIMP asks how to read the file (so, going with normal initial settings). Go to “File” and choose “Export As” and choose JPG/PDF (depending on the file, if drawing or photo, choose JPG. Flyer design choose PDF). Slide the resolution up to 10 and hit “Export” and navigate to proper folder for it to export to. 
5. If you run into an odd or unfamiliar file type, contact the digital archivist for assistance

*To stay in BitCurator/Ubuntu:*
1. Use *convert scripts* in BitCurator – ASK ZL TO WRITE OUT COMPREHENSIVE README FOR THIS

[Back to top](#table-of-contents)

---

## Arranging Files
WRITE THESE

[Back to top](#table-of-contents)

---

## TAR Files
1. In [collectionName]_workingFiles, create a folder called [MSS]files
2. Create TAR files for the Original Disk Images and the Working Files folders </br>
•	Create TAR file containing both of these folders/files following [these instructions](https://bedwards254.github.io/testBDBC/jekyll/2019/01/29/TAR-files.html)
3. Put this TAR file in the [MSS]files folder, along with a copy of the MD5 file created above

[Back to top](#table-of-contents)

---

## Bagging Files
*Switch to Ubuntu if not already in it, [using these instructions](https://bedwards254.github.io/testBDBC/jekyll/2019/01/22/BC-Windows-Switch.html)*
1. In BitCurator, mount the hard drive and navigate to the [collectionName]_workingFiles folder
2. Right click inside the folder and select “Open in Terminal”
3. In the terminal, type `bagger.py –md5 –sha1 –contact-name=[netID] ./[MSS]files`
4. Let it run
5. Once it is done running, in the terminal, type `bagger.py –validate ./[MSS]files`
6. A message should appear saying it is valid </br>
•	If not, contact the digital archivist</br>

[Back to top](#table-of-contents)

---

## Uploading to Keep
*Staff: Follow these instructions to upload the bagged file into the Keep: https://bedwards254.github.io/testBDBC/jekyll/2019/01/22/Keep-Ingest.html*
1. **Abstract:** *TAR file of files brought to Tier 2 processing, MD5 file, and original disk image*
2. **Imaging Date:** put the date the bag was created
3. **Hardware:** put the summation of the media, without count
4. **Other Information:** put *Originally [number of media (six optical discs, 120 3.5” floppy disks, etc.); summation of collection.*

[Back to top](#table-of-contents)

---

## Directory Listing
WRITE THIS

[Back to top](#table-of-contents)

---

## Finding Aid Edits
WRITE THESE

[Back to top](#table-of-contents)

---

## Upload to Reading Room Server
WRITE THESE

[Back to top](#table-of-contents)
