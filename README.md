# SMRTlinkSingularity
singularity image definition for SMRT link v11

Definition file for the creation of a singularity image containing SMRTlink v11
The image created is large (> 4Go). Make sure you

How to:

    install singularity on your machine (or WM) and make sure you have the sudo rights

    To build the image:

     sudo singularity build SMRTlinkv11.sif SMRTlinkv11.def

    To use the image in an interactive shell:

     singularity shell SMRTlinkv11.sif 

    execute a specific tool:

     singularity exec SMRTlinkv11.sif bamsieve input.bam --show-zmws

Enjoy!
