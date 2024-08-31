# FEMM to LTspice Automation
A python based automation transfering data from FEMM to LTspice.\
This project provides an automated environment using Python and Jupyter Notebook for intuitive documentation and execution of the process.\ 
The automation environment is developed for a Toroidal coil magnetic component and its application in a Boost converter. Adjustments may be needed to support different geometric components.

## Installation Instructions

### 1. Install Anaconda
Anaconda is a distribution of the Python and R programming languages for scientific computing, that aims to simplify package management and deployment. (Wikipedia)\
While using Anaconda is not mandatory, it facilitates the initial setup and configuration of the environment, making it simple to start with.\
Anaconda is available on some of the faculty computers. If not already installed, follow these steps:

1. Download Anaconda from [Anaconda's website](https://www.anaconda.com/).
   - Click on "Free Download" (top right corner).
   - Optionally, skip registration.
   - Choose the download according to your operating system (for Windows: [Anaconda3-2024.06-1-Windows-x86_64.exe](https://repo.anaconda.com/archive/Anaconda3-2024.06-1-Windows-x86_64.exe)).
2. Installation: Open the downloaded installer and follow the on-screen instructions.

### 2. Install Python Libraries

You can install the required Python libraries using Anaconda's CMD prompt:

1. Open Anaconda Prompt (CMD.exe).
2. Run the following command to install the necessary libraries:
   ```bash
   pip install pyfemm ltspice
3. Wait for the installation to complete and then close the terminal.

### 3. Initial File Setup

For initial setup, work within a single directory located in Anaconda's path. You can later adjust file locations and paths in the code as needed.

1. Navigate to the installation path:
   - the default is something like: C:\Users\<your_user>\anaconda3\
2. Create a new directory, e.g.  <femm_to_LTspice>.
3. Clone the project repository and place the notebook in the new directory:
   - Git Repository: GitHub - FEMM_to_LTspice
   - Notebook File: FEMM_to_SPICE_notebook_V0.ipynb
   - Path: C:\Users\<your_user>\anaconda3\femm_to_LTspice
4. For initial execution, download additional files and move them to the directory:
   - Boost_Converter_V0.asc
   - Boost_Converter_V0.raw
   - toroid_core_geometry_V0.ans
   - toroid_core_geometry_V0.fem
   - Ferrite_N87_BH_Curve.dat
5. To work with the Boost converter example, add the comparator symbol files (you can place in the same directory):
   - Ideal_Comparator.asy
   - Ideal_Comparator.sub
6. Optionally, if using your own FEMM model, place it and its analysis results in this directory:
   - <femm_file>.ans
   - <femm_file>.fem
   - For LTspice simulation files, also add <spice_file>.asc, <spice_file>.raw

### 4. Open the Notebook and Start Working
Note: Ensure FEMM and LTspice are already installed on your computer before proceeding.

1. FEMM can be downloaded from [FEMM's website](https://www.femm.info/wiki/Download) (64-bit Executable)

2. LTspice can be downloaded from [LTspice's website](https://www.analog.com/en/resources/design-tools-and-calculators/ltspice-simulator.html) and installed using (LTspice64.msi).

3. Launch Anaconda.

4. Open Jupyter Notebook (or Jupyter Lab) from Anaconda.

5. Navigate to the notebook file (FEMM_to_SPICE_notebook_V0.ipynb) and open it.
   - Path is something like: C:\Users\<your_user>\anaconda3\femm_to_LTspice

6. Follow the instructions in the notebook.\
It is recommended to run each cell individually to ensure proper functionality without errors. Make necessary adjustments to paths, filenames, and model values as needed.
