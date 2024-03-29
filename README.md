# Lysosome analysis

This is a set of scripts to classify and track lysosomes of different shapes. 
The input data is a thresholded image stack of moving lysosomes which have different
shapes and move with different speeds depending on their shape.

The script classifies lysosomes into two categories, spheres and tubes, and then uses the Crocker and Grier
algorithm (Crocker and Grier, 1996) in a MATLAB implementation to track the spherical and tubular particles individually.

![Lysosomes](images/lysosomeClassification.jpg)

The average displacement and velocities for the particles are extracted and plotted, and .csv files with the 
tracks and the velocities are also extracted for plotting in R. 
