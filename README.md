# Smart-Cropping

Using Python, this script will convert PDF to image files to a given location, 1 image for each page of the PDF.
Then it will iterate each image of that location and crop each side of the images based on reference background color and then
insert images into Excel.  Note, this was created specifically for my needs.  
I removed all the file locations i use from the script, so you will have to enter those in yourself.
Use what you want from it.


Note:  The way the Smart cropping works is by reading the background color, then iterates through the TOP/SIDES/BOTTOM pixels
each separately until it finds an RGB value significately different from the background color and sets that location
for the crop.

Note #2:  This uses PyQt5 GUI.  You enter in the filename of the PDF you want the script to work on and it auto finds the file
within the given pathway listed in the "balloned_folder" variable pathway.


![image](https://user-images.githubusercontent.com/123666150/214939533-1819d362-b238-447d-bc32-7242d783992e.PNG)
