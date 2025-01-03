### Introduction

This is a repository for analysis of the growth of PTCDI-C8 thin layer recorded with quick X-ray reflectivity (XRR) measurement. We used Neural Network as the main analysis tool together with refnx fitting algorithm. This approach is chosen for its convenience and speed compared to advanced genetic algorithms, particularly when dealing with a large dataset of 10,000 curves generated during the growth of the thin film.

### Data folders:

`data_evolution` - predicted labels from all experiments
`data_evolution_error` - predicted labels from all experiments with extracted averages and error bars
`inter` - qXRR curves for the growth at 0.2 nm/s
'interS' - qXRR curves for the growth at 0.1 nm/s   

### Model:

'DensNet_PTCDI' - model
'normalization_PTCDI.npy' - labels normalization

'Data_generator.ipynb' - training data generation using refnx ('labels.npy' and 'curves.npy')
'Data_augmentation.ipynb' - data augmentation script ('labels_N.npy' and 'curves_N.npy')
'Training.ipynb' - This notebook demonstrates the training of a neural network using a generated dataset. A minimal training dataset is included to illustrate the fundamental principles of the training process.

### Python scripts:

'BP_fit.py' - refnx fit and image generator
'BP_fit_multi.py' - refnx fits and images generator

### Text files:

'bragg_intensities.txt' - extracted intensities of the Bragg peak during the growth
'Pilatus_Interpolated.txt' - measured XRR curve with a classical XRR setup after the growth at 0.1 nm/s

### Notebooks:

'Prediction_fit_single.ipynb' - NN and NN-informed fit of an XRR curve (Figure 1 in the main text)
'Prediction_fit_multiple.ipynb' - NN and NN-informed fit of an XRR curve (Figure 2 in the main text)
'Thin_film_evolution.ipynb' - analysis of the growth of the thin layer at the growth rate of 0.1 nm/s (Figure 2 in the main text)
'Prediction.ipynb' - NN prediction of the labels for the experimental data (growth at 0.2 nm/s)
'refnx_fit.ipynb' - script for refnx fit
'Plot_Final.ipynb' - A 3D plot depicting the double exponential function fitted to the roughness evolution of the thin film using the complete experimental dataset (Figure 3 in the main text).  
'Plot_Final_error.ipynb' - A 3D plot illustrating the double exponential function fitted to the roughness evolution of the thin film, based on the average experimental data (Figure S12 in the SI). Additionally, an analysis of the thickness of the coherently ordered fraction of the thin film as a function of molecular exposure is presented (Figure 4 in the main text).


If you have any questions or suggestions, please don't hesitate to reach out.




