# Tier 2
Tier 2 processing is done by staff, students, and interns as deemed appropriate. 

[instert steps here as ToC]

## Folder Structure Setup
1. Create a folder called [collectionName]_workingFiles
2. Inside of that folder, create 3 folders called: 
a. Original Disk Images;
b. Extracted Files; and
c. Working Files
3. In Original Disk Images, create folders for each disk image you’re pulling down from the Keep
4. Copy the folders you just made to Extracted Files

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


## Virus Scanning
1. Once the files are extracted, select all of the folders in the Extracted Files folder (Ctrl+A)
2. Right click and select “Scan with McAfee Virus Defense”
3. A window will pop up showing how many files are being scanned
4. When done, it will say “Scan: Complete” and have a count of infected files below
5. If any files are infected, let the digital archivist know right away

Copy the files in Extracted Files to Working Files

## Switching to BitCurator/Ubuntu from Windows
1. [Instructions here](https://bedwards254.github.io/testBDBC/jekyll/2019/01/22/BC-Windows-Switch.html) 
2. Eject the hard drive before doing this step, and turn off the hard drive dock OR disconnect the USB cable 
3. Shut down the computer fully when switching between the two


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


## MD5 File Creation
*Create MD5 file for Working Files folder*
1. Select all the folders in Working Files
2. Right click and select “Scripts” and then “Calculate MD5 script”
3. A pop-up box will appear showing the progress
4. Once done, a file called md5 will appear in the main Working Files folder
5. Open it to check the contents


## Duplication Detection
### FSLint


## TAR Files


## Bagging Files


## Uploading to Keep
