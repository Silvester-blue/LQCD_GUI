# LQCD_GUI

Introduction
============
A graphical user interface (GUI) software is provided for lattice QCD simulations, aimed at streamlining the process. The current version of the software employs the Metropolis algorithm with the Wilson gauge action. It is implemented in Python, utilizing Just-In-Time (JIT) compilation to enhance computational speed while preserving Python's simplicity and extensibility. Additionally, the program supports parallel computations to evaluate physical quantities at different inverse coupling $\beta$ values, allowing users to specify the number of CPU cores. The software also enables the use of various initial conditions, as well as the specification of the save directory, file names, and background settings. Through this software, users can observe the configurations and behaviors of the plaquette under different $\beta$ values.

Usage Instructions
============

In the GUI, set the required parameters (**lattice size**, $\beta$, iteration counts, CPU core numbers, and initialization scheme).

1. **Lattice Size**: The lattice size supports two input methods. When \(N_x = N_y = N_z\), only \(N_t\) and \(N_x\) need to be specified. The program will automatically interpret these as \(N_t\), \(N_x\), \(N_y\), and \(N_z\). In this example, the input ``8,4'' indicates \(N_t = 8\) and \(N_x = N_y = N_z = 4\). If \(N_x\), \(N_y\), and \(N_z\) are not equal, all four parameters must be provided, separated by commas.

2. **$\beta$**: Multiple values for \(\beta\) can be input simultaneously to facilitate parallel computations. Different values should be separated by commas.

3. **Iteration Counts**: One complete update of all lattice points is called one sweep. Furthermore, it is computationally economical to repeat the updating step 10 times for the visited variable, since the computation of the sum of staples is costly\cite{Gattringer2010}. In this context, one iteration corresponds to 10 sweeps.

4. **Initialization Scheme**: The default option is a cold start; however, users can also select a hot start.

5. **File Saving Options**: Users can specify the save directory and file name. In this example, if the file name is designated as ``Test'', all file names of generated configurations and plaquette-related files will begin with ``Test''.

After completing these parameter settings, press the ``Run Simulation'' button to initiate the simulation.


Example
============
<p align="center">
    <img src="images/Ising_test.jpg"  width="500"/>
</p>
    
<p align="center">
    <i>An example of software parameters</i>
</p>

