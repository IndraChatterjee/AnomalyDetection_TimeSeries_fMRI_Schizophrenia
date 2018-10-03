# AnomalyDetection_TimeSeries_fMRI_Schizophrenia

### By: Indranath Chattterjee
### Department of computer science, University of Delhi, Delhi-110007,
### E-mail: indranath.cs.du@gmail.com

#### IndraChatterjee/AnomalyDetection_TimeSeries_fMRI_Schizophrenia is licensed under the Creative Commons Attribution 4.0 International


Run the code in the following order:


Step 1. Run the 'script_dataload.m' locating the proper directory containing all the runs of the preprocessed time-series fMRI data.


Step 2. Run the 'intersection_union_script.m'


Step 3. If want to classify with SVM, run 'classification_SVM.m', and if with ELM then run 'classification_ELM.m'


The MAT file named 'Contrast_AudOdd_Dev_Std_15T_2D.mat' contains the data for 34 healthy subjects (first 34) and 34 schizophrenia patients (next 34).
This are the contrast maps obtained from GLM analysis of time-series fMRI data for 4 runs of Auditory-oddball task.
Each row contains the 153594 voxels covering the whole brain for each subject. The 4 runs of each subject's data are averaged.


1) This program will fetch the time-series fMRI data of each of the 4 runs of 
the Auditory-oddball (AUD) task for each of the 34 healthy subjects 
and 34 schizophrenia patients. 

2) This program will try to find the changes in the activation pattern 
within a particular voxel along its time-series with the help of 
mean-deviation based analysis.

3) Using the simple set operations, the index of the relevant brain voxels will be obtained.

4) This index file can be fed as as input to classifier as a feature set during building the classification model.



