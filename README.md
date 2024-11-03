# LQCD_GUI

Introduction
============
A graphical user interface (GUI) software is provided for lattice QCD simulations, aimed at streamlining the process. The current version of the software employs the Metropolis algorithm with the Wilson gauge action. It is implemented in Python, utilizing Just-In-Time (JIT) compilation to enhance computational speed while preserving Python's simplicity and extensibility. Additionally, the program supports parallel computations to evaluate physical quantities at different inverse coupling \(\beta\) values, allowing users to specify the number of CPU cores. The software also enables the use of various initial conditions, as well as the specification of the save directory, file names, and background settings. Through this software, users can observe the configurations and behaviors of the plaquette under different \(\beta\) values.

Usage Instructions
============

1.Running the Simulation:

Input the desired parameters (lattice size, temperatures, iterations, etc.) into the GUI fields.
Press the Run Simulation button to start the process. In addition, this software supports parallel computing, and you can specify the number of CPU cores yourself.

2.Customization:

Background image can be customized by replacing the background.jpg file used in the GUI.

3.Data Saving:

Results, including final lattice states and magnetization data, are automatically saved in the specified directory.


Example
============
<p align="center">
    <img src="images/Ising_test.jpg"  width="500"/>
</p>
    
<p align="center">
    <i>An example of software parameters</i>
</p>

