Overview 

Description: The goal of this project aims to use a neural network to model and optimize beam steering in the Linac to Undulator (LTU) section of the LCLS to minimize beam offsets at the BPMs. 
The neural network will represent a function mapping the following inputs to the output beam

Inputs:
● Quadrupole magnet strengths (k1, k2, ..., kN)
● Corrector magnet settings (c1, c2, ..., cM)
● Beam energy (E)
Output:
● Beam position monitor (BPM) offsets (x1, x2, ..., xP)

