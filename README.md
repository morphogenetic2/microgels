# Microgel image analysis
 This is a simple python script to analyze brightfield/phase contrast images of mostly spherical microparticles or microgels.

 ## Setup Instructions

1. Install Miniconda or Anaconda if you haven't already. Miniconda is highly recommended, you can install it from [here](https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe). Requires administrator privileges.

2. Clone this repository or download the script and environment.yml file. You can clone the repository by installing git on your computer and typing
   ```
   git clone https://github.com/morphogenetic2/microgels.git
   ```


3. Open a terminal or command prompt and navigate to the directory containing the files.

4. Create the conda environment using the following command:
   ```
   conda env create -f environment.yml
   ```

5. Activate the environment:
   ```
   conda activate microgel-analysis
   ```

6. Run the script:
   ```
   jupyter notebook analysis.ipynb
   ```

7. The jupyter notebook will show up in your default browser (probably Chrome) and you only need to press the ▶ button on the toolbar.

## Howto

1. Select the folder containing your images using the file chooser. The images must be in .tiff or .png format.
2. Enter the estimated diameter (in pixels) of the microgels. You can estimate it quickly using the measure tool in ImageJ.
3. Click the "Process Images" button to start the analysis.
4. The script will generate mask overlays and save them in the "mask_overlays" subfolder.
5. Segmentation results will be saved as an Excel file in the selected folder. By default, and to avoid artifacts, the script will only save the segmented masks with an aspect ratio between 0.8 and 1.2, but this can be easily modified in the script.
