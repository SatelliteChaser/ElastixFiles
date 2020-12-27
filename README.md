# ElastixFiles

Files for aligning RGB images of the moon to an L(or something else) frame. To use them, copy the files to where elastix is installed.

The bat file can be used to automatically align all three frames to the reference, just edit the paths and create the destination folders, then doubleclick on the bat file. The resulting files will  be located in the subfolders proc/R, proc/G, proc/B. Result.0.png will be the image where only translation and rotation is performed, result.1.png will also have non rigid transformation (pixels will be moved without restriction).

The rigid.txt  does only rotation and translation, the nonrigid.txt moves pixels without restrictions.

Key parameters in the parameter files are:

* (MaximumNumberOfIterations x x x x) : Lower this to increase speed at the cost of accuracy.
* (FinalGridSpacingInPhysicalUnits x) : Decrease to allow for bigger non rigid transformation, increase to force smaller non rigid transformations. Tweak this if you get wrong warps.

General tips:

* Crop as much background as possible
* The input file needs to be 16 bit, otherwise the output will be a blank image.
