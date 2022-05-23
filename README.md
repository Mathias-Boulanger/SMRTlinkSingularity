# SMRTlinkSingularity
Singularity image definition for SMRT link v11

Definition file for the creation of a singularity image containing SMRTlink v11.0.0.146107
The image created is large (> 4Go). Make sure you have enough storage when creating the image.

How to:

#install singularity on your machine (or WM) and make sure you have the sudo rights
##To build the image:

    sudo singularity build SMRTlink_v11.sif SMRTlink_v11.def

##To use the image in an interactive shell:

     singularity shell SMRTlink_v11.sif 

##To execute a specific tool:

     singularity exec SMRTlink_v11.sif bamsieve input.bam --show-zmws

Enjoy!
