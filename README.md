This macro combines a few different small macros I created for basic pre-processing:

-Blind -> takes a folder of images, assigns them a random number name, saves a copy in a new folder + prints out the name of the image next to the random number code. This version will spit out names in a name-1, name-2, number-1, number-2 format because it was intended to go along with a protocol that required selection of two dendrites from a single image and it reduced the amount of time I needed to spend renaming all of the single image blinds.

-Select Dendrites -> takes a stack of opened images and automates a framework in which two dendrites will be selected and measured for length per image. It will ask if there are usable dendrites in frame, and if the response is "yes", will continue, if it is anything but "yes" it will close the image and move to the next one. Once selected, the dendrites will automatically save in the noted folder and the ROI outline and length will be saved in a separate noted folder. The macro will print out the name of the image with a "-1" or "-2" and the length of each dendrite

-Unblind -> takes images from a folder and renames them, used to convert the blinded dendrites to unblinded prior to introduction to the dendrite analysis macro which requires a threshold set from the control condition and subfolders with each condition.

-Split Channels for Thresholding -> takes a stack of open images(RGB), splits it into three channels, inverts them, automates the selection of thresholds for the red and green channels for each image, and prints out the result with the number correction for the color inversion.

-non-puncta analysis Blind -> the same thing as "Blind" without the extra formatting of the results. 

-Triple Thresholding -> the same thing as "Split Channels for Thresholding" except it adds the blue channel as well.
