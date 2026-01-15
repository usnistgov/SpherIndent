# SpherIndent: An open-source Python software for calibration, analysis and visualization of spherical nanoindentation experiments

## Description

<p style="text-align: justify;">SpherIndent is a modular, open-source software package with graphical user interface (GUI) for analysis of quasi-static spherical indentation experiments conducted in single-step or multi-step loading sequences. </p><p style="text-align: justify;">All components are developed in Python programming language with the GUI built on Tkinter. The software package is essentially constructed using libraries including NumPy, Pandas, SciPy, Sklearn, Matplotlib, and OpenCV. Data storage, from raw to processed and analyzed data (including figures) is handled via Pickle with traceability, efficient retrieval and sharing in mind. SpherIndent only uses tabular data from indentation experiments (time-depth-force), image files from peripheral equipment (i.e., scanning electron microscopes – SEM-), or self-generated files. </p> 
<p style="text-align: justify;">SpherIndent includes:</p> 
<ul>
  <li>calibration routines to determine machine compliance based on indentation of reference materials, </li>
  <li>calibration routines to determine the tip geometry (i.e., tip radius and cone angle) via tip-area function calculation or tip image analysis,</li>
  <li>data conditioning routines to eliminate thermal drift, compute zero-point offset, and correct for machine compliance effects,</li>
   <li>analysis routines to extract various material metrics of interest (e.g., Hertz and Oliver-Pharr elastic moduli, dissipation indices, maximum shear stress at first pop-in, stress-strain pairs) from SII and MSI indentation tests.</li>
</ul>

</p>For full details on the initial version of SpherIndent, please consult the associated peer-reviewed publication[[1]](#references).

## Table of Contents

* [Setup](#setup)
* [Usage](#usage)
* [Example](#example)
* [Notes](#notes)
* [License and Disclaimer](#license-and-disclaimer)
* [Contact](#contact)
* [References](#references)

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

## Example
Examples are provided in the associated peer-reviewed publication [[1]](#references). The examples leverage the public dataset in [[2]](#references).

## Notes
Certain commercial equipment, software, instruments, and materials are identified in this document. Such identification does not imply recommendation or endorsement by the National Institute of Standards and Technology, nor does it imply that the products identified are necessarily the best available for the purpose. 

## License and Disclaimer
This software was developed by employees and contractors of the National Institute of Standards and Technology (NIST), an agency of the Federal Government and is being made available as a public service. Pursuant to title 17 United States Code Section 105, works of NIST employees are not subject to copyright protection in the United States. This software may be subject to foreign copyright. Permission in the United States and in foreign countries, to the extent that NIST may hold copyright, to use, copy, modify, create derivative works, and distribute this software and its documentation without fee is hereby granted on a non-exclusive basis, provided that this notice and disclaimer of warranty appears in all copies.

THE SOFTWARE IS PROVIDED 'AS IS' WITHOUT ANY WARRANTY OF ANY KIND, EITHER EXPRESSED, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY THAT THE SOFTWARE WILL CONFORM TO SPECIFICATIONS, ANY IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND FREEDOM FROM INFRINGEMENT, AND ANY WARRANTY THAT THE DOCUMENTATION WILL CONFORM TO THE SOFTWARE, OR ANY WARRANTY THAT THE SOFTWARE WILL BE ERROR FREE. IN NO EVENT SHALL NIST BE LIABLE FOR ANY DAMAGES, INCLUDING, BUT NOT LIMITED TO, DIRECT, INDIRECT, SPECIAL OR CONSEQUENTIAL DAMAGES, ARISING OUT OF, RESULTING FROM, OR IN ANY WAY CONNECTED WITH THIS SOFTWARE, WHETHER OR NOT BASED UPON WARRANTY, CONTRACT, TORT, OR OTHERWISE, WHETHER OR NOT INJURY WAS SUSTAINED BY PERSONS OR PROPERTY OR OTHERWISE, AND WHETHER OR NOT LOSS WAS SUSTAINED FROM, OR AROSE OUT OF THE RESULTS OF, OR USE OF, THE SOFTWARE OR SERVICES PROVIDED HEREUNDER.

## Contact
Please contact Nicolas A. Alderete (nicolas.alderete@nist.gov, [ORCID: 0000-0002-2145-8825](https://orcid.org/0000-0002-2145-8825) or Yvonne B. Gerbig (yvonne.gerbig@nist.gov, [ORCID: 0000-0002-8947-4215](https://orcid.org/0000-0002-8947-4215))

## References
[1] Alderete, N.A., Gerbig, Y.B., *SpherIndent: An open-source python software for calibration, analysis and visualization of spherical nanoindentation experiments*, Journal. [doi: 0.18434/Mds2-4051](https://doi.org/0.18434/Mds2-4051).<br>
[2] Gerbig, Y.B., Alderete, N.A., *Demonstration dataset for open-source SpherIndent analysis and calibration software for spherical nanoindentation experiments*, NIST Public Data Repository, [doi: 0.18434/Mds2-4051](https://doi.org/0.18434/Mds2-4051).
