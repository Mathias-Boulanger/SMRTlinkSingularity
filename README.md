# SMRT link Singularity image definition

Definition file for the creation of a singularity image containing SMRTlink v11.0.0.146107.
The created image is large (> 4Go). Make sure you have enough storage space when creating the image.

How to proceed:

- install singularity on your machine (or WM) and make sure you have the sudo rights
- To build the image:

        sudo singularity build SMRTlink_v11.sif SMRTlink_v11.def

- To use the image in an interactive shell:

        singularity shell SMRTlink_v11.sif 

- To execute a specific tool:

        singularity exec SMRTlink_v11.sif bamsieve input.bam --show-zmws

To mount specific repo accessible by the singularity image, you can set up this variable once: `export SINGULARITY_BINDPATH=/opt,/MYPATH` 

The definition file 'SMRTlink_v11_full.def' contains extra installed tools listed below:
- bedops suite
- bedtools suite
- GNU datamash

Enjoy!
