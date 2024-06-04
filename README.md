# ga_IRST_repo


# Overview
This codebase is written entirely in python, and includes scripts to parse the inputed CALIPSO datafiles, manipulate the extracted data arrays, and simulate visibility/cloud cover statistics within these datafiles.

# CALIPSO Dataset

The CALIPSO project is a NASA satteline project that takes 3D strip measurements of Earth's atmosphere. For more detailed information just go to their website which I have linked in the Resources section. For the purposes of this simulation a couple things are worth noting here.
1) The measurements that are taken by the sattelite are strip measurements, meaning that although their is a physical 3D space that the data corresponds to, the actual data arrays from the CALIPSO database are reported as 2D arrays (acknowledging that their is actually some width to that 2D array. This means that if we want to characterize a whole region, we need to use a large dataset (hundreds, potentially thousands of seperate CALIPSO files) to accuratley reconstruct the behavior of a broad region.

# How to Run

1) Pull this Repository into your Desktop
2) Make a folder called CALIPSO_VFM_Data and put it in the folder titled VFM_Simulation
3) Open the file called "FileManager_IRST.py" in VS Code or you editor of choice
4) Run and wait for output : should be a png graph of the dataset in the file specified in the simulation main file as well as statistical summary of the simulation. You can check to see if it looks right by plotting in ccplot or VOCAL, or on the CALIPSO main website (First Link), NASA publishes images of all the datasets that are publically available so you can also visually inspect the CALIPSO dataset that way.

# Useful/Related Resources
1) https://www-calipso.larc.nasa.gov/resources/calipso_users_guide/   |   CALIPSO User Guide Homepage
2) http://hdfeos.org/zoo/index_openLaRC_Examples.php#CALIPSO    | HDF_EOS example parsing and visualisation of CALIPSO files
3) http://fhs.github.io/pyhdf/index.html  |   documentation for pyhdf python module for reading and parsing HDF files
4) https://ccplot.org/   |  CCPLOT, tool for visualizing CALIPSO data ---- similair tool called VOCAL, which uses ccplot and has some additional GUI attached (problem is that it runs using Python 2.7, and probably has some wack package and code dependencies that might be more trouble than it's worth --- caveat I haven't actually tried using VOCAL)

# Contact

Feel free to use whatever code you want, I try to generally comment out my code as well as I can, but (disclaimer), I'm a Physics guy not a CS guy so if you want any help on deciphering my code, or any associated questions about how to use the code you can contact me at (619)306-8830. Or if you prefer email my email is pvollrath392@gmail. 
