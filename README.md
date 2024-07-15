# CUDA at Scale Independent Project

## Description

This program applies CUDA box filters to all images in a folder, using NPP's `nppiFilterBoxBorder_8u_C1R` routine.

(Based on nvidia's sample code: https://github.com/NVIDIA/cuda-samples/tree/master/Samples/4_CUDA_Libraries/boxFilterNPP)

## Implementation Details

`boxFilterNPP.cpp` is the main implementation, it loops through all files in the input folder, reads the image,
copies to device, applies the filter, and writes the result to the output folder.

`Common` contains the helper code for error checking and image file handling.

`data` contains example input images.

`output` contains output for the example inputs.

`Makefile` for compiling the code.

`run.sh` contains scripts for building the code and running on example inputs.

## Running the Program

Run the following command, with the `-input` flag to specify the input folder to use:
  ```bash
  run.sh
  ```
