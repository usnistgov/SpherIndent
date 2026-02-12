# SpherIndent: An open-source Python software for calibration, analysis and visualization of spherical nanoindentation experiments

## Description

<p style="text-align: justify;">SpherIndent is a modular, open-source software package with graphical user interface (GUI) for analysis of quasi-static spherical indentation experiments conducted in single-step or multi-step loading sequences. </p><p style="text-align: justify;">All components are developed in Python programming language with the GUI built on Tkinter. The software package is essentially constructed using libraries including NumPy, Pandas, SciPy, Sklearn, Matplotlib, and OpenCV. Data storage, from raw to processed and analyzed data (including figures) is handled via Pickle with traceability, efficient retrieval and sharing in mind. SpherIndent only uses tabular data from indentation experiments (time-depth-force), image files from peripheral equipment (i.e., scanning electron microscopes – SEM-), or self-generated files. </p> 
<p style="text-align: justify;">SpherIndent includes:</p> 
<ul>
  <li>Calibration routines to determine machine compliance based on indentation of reference materials, </li>
  <li>Calibration routines to determine the tip geometry (i.e., tip radius and cone angle) via tip-area function calculation or tip image analysis,</li>
  <li>Data conditioning routines to eliminate thermal drift, compute zero-point offset, and correct for machine compliance effects,</li>
  <li>Analysis routines to extract various material metrics of interest (e.g., Hertz and Oliver-Pharr elastic moduli, dissipation indices, maximum shear stress at first pop-in, stress-strain pairs) from SII and MSI indentation tests.</li>
</ul>

## Table of Contents

* [Setup](#setup)
* [Usage](#usage)
* [Examples](#examples)
* [Notes](#notes)
* [Funding](#funding)
* [License and Disclaimer](#license-and-disclaimer)
* [Contact](#contact)
* [References](#references)
* [Related Materials](#related-materials)

## Setup

### Using Conda

1. Create a Conda environment from the provided 'spherindent_env.yml file:
   conda env create -f spherindent_env.yml -n [your_env_name]
2. Activate the environment:
   conda activate [your_env_name]

### Using pip

1. Create a Conda environment from the provided 'spherindent_env.yml file:
   conda env create -n [your_env_name]
2. Activate the environment:
   conda activate [your_env_name]
2. Install dependencies:
   pip install -r requirementsSpherIndent.txt

## Usage

To run this code, follow these steps:

### Using Spyder

1. Open Spyder and create a new project or open an existing one.
2. Open the spherIndent.py script.
3. Make sure you select the Conda environment created earlier in Tools>Preferences>Python Interpreter.
4. Make sure you change the plotting of your Spyder from inline to automatic (inline exhibits odd behavior).Tools>Preferences>IPython console>Plotting>Graphics backend>Automatic
4. Run the script by clicking on the "Run" button or pressing F5.
5. Use the GUI.

### Using VSCode

1. Open VSCode and open the folder containing your project.
2. Make sure you have the Python extension installed.
3. Open the spherIndent.py script.
4. Make sure you have selected the correct Python interpreter (i.e., the one from your Conda environment) by clicking on the Python version in the bottom left corner of the VSCode window.
5. Run the script by clicking on the "Run Code" button or pressing F5.
6. Use the GUI.

Alternatively, you can also run the script from the terminal/command prompt:

python spherIndent.py

## Examples
Examples are provided in the associated peer-reviewed publication [[1]](#references). The examples leverage the public dataset in [[2]](#references).

## Notes
Certain commercial equipment, software, instruments, and materials are identified in this document. Such identification does not imply recommendation or endorsement by the National Institute of Standards and Technology, nor does it imply that the products identified are necessarily the best available for the purpose. 

## Funding
This work was performed with funding from the CHIPS Metrology Program, part of CHIPS for America, National Institute of Standards and Technology, U.S. Department of Commerce.

## License and Disclaimer
NIST-developed software is provided by NIST as a public service. You may use, copy, and distribute copies of the software in any medium, provided that you keep intact this entire notice. You may improve, modify, and create derivative works of the software or any portion of the software, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the software and should note the date and nature of any such change. Please explicitly acknowledge the National Institute of Standards and Technology as the source of the software. 

NIST-developed software is expressly provided "AS IS." NIST MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED, IN FACT, OR ARISING BY OPERATION OF LAW, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT, AND DATA ACCURACY. NIST NEITHER REPRESENTS NOR WARRANTS THAT THE OPERATION OF THE SOFTWARE WILL BE UNINTERRUPTED OR ERROR-FREE, OR THAT ANY DEFECTS WILL BE CORRECTED. NIST DOES NOT WARRANT OR MAKE ANY REPRESENTATIONS REGARDING THE USE OF THE SOFTWARE OR THE RESULTS THEREOF, INCLUDING BUT NOT LIMITED TO THE CORRECTNESS, ACCURACY, RELIABILITY, OR USEFULNESS OF THE SOFTWARE.

You are solely responsible for determining the appropriateness of using and distributing the software and you assume all risks associated with its use, including but not limited to the risks and costs of program errors, compliance with applicable laws, damage to or loss of data, programs or equipment, and the unavailability or interruption of operation. This software is not intended to be used in any situation where a failure could cause risk of injury or damage to property. The software developed by NIST employees is not subject to copyright protection within the United States.

To see the latest statement, please visit: [Copyright, Fair Use, and Licensing Statements for SRD, Data, Software, and Technical Series Publications](https://www.nist.gov/open/copyright-fair-use-and-licensing-statements-srd-data-software-and-technical-series-publications#software)

## Contact
Please contact Nicolas A. Alderete (nicolas.alderete@nist.gov, [ORCID: 0000-0002-2145-8825](https://orcid.org/0000-0002-2145-8825) or Yvonne B. Gerbig (yvonne.gerbig@nist.gov, [ORCID: 0000-0002-8947-4215](https://orcid.org/0000-0002-8947-4215)) for questions.

## References
[1] Alderete, N.A., Gerbig, Y.B., *SpherIndent: An open-source python software for calibration, analysis and visualization of spherical nanoindentation experiments*, (Under review). [doi: 0.18434/Mds2-4051](https://doi.org/0.18434/Mds2-4051).<br>
[2] Gerbig, Y.B., Alderete, N.A., *Demonstration dataset for open-source SpherIndent analysis and calibration software for spherical nanoindentation experiments*, NIST Public Data Repository, [doi: 0.18434/Mds2-4051](https://doi.org/0.18434/Mds2-4051).

## Related Materials
The work was done under the CHIPS project [Characterization of Nano-to-Microscale Process-Induced Thermo-Mechanical Changes in Heterogeneously Integrated Microelectronics](https://www.nist.gov/programs-projects/characterization-nano-microscale-process-induced-thermo-mechanical-changes)
