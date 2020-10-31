# ElastixFiles

Files for aligning RGB images of the moon to an L(or something else) frame. To use them, copy the files to where elastix is installed.

The bat file can be used to automatically align all three frames to the reference, just edit the paths and create the destination folders, then doubleclick on the file. The resulting files will all be called result.1.png, and they will be located in the subfolders proc/R, proc/G, proc/B.

The rigid.txt  does only rotation and translation, the nonrigid.txt moves pixels without restrictions.
