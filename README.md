# Clustering Lab – Fisher Iris Dataset
Clustering Lab – Fisher Iris Dataset

This repository contains my work for CS-345/M45 Lab Class 2, focused on applying unsupervised learning methods to the classic Fisher Iris dataset. The exercises walk through k-means, Gaussian Mixture Models (GMMs), visualisation of soft and hard cluster assignments, and clustering an unknown dataset.

Repository Structure
├── <student-number>-Clustering.ipynb   # Main notebook with all tasks
├── Iris_data.npy                      # Feature data (4-dimensional)
├── Iris_labels.npy                    # True species labels
└── task2-4.npy                        # Unlabelled dataset for Task 2.4

Overview

The notebook explores clustering through progressively more advanced tasks:

Task 2.1 – Exploring the Fisher Iris Dataset

Loads Iris_data.npy and Iris_labels.npy.

Introduces the dataset in markdown.

Visualises the dataset using scatter plots coloured by the true labels.

Discusses feature dimensions, number of samples, and class labels.

Task 2.2 – k-Means Clustering

Builds a k-means model using scikit-learn’s KMeans class.

Fits the model using all four features.

Predicts cluster assignments and visualises the results.

Adds centroids to the plot.

Experiments with parameters such as init and n_init.

Task 2.3 – Gaussian Mixture Models (GMMs)

Implements clustering with scikit-learn’s GaussianMixture.

Fits the model and compares predicted clusters with true labels and k-means clusters.

Plots Gaussian component means.

Computes and visualises posterior probabilities for each component.

Produces intensity maps showing soft clustering behaviour.

Tests different initialisation strategies (init_params, etc.) to improve results.

Task 2.4 – Clustering an Unknown Dataset

Loads the dataset from task2-4.npy.

Applies the techniques from earlier tasks to estimate the underlying number of clusters.

Includes visualisations and reasoning rather than focusing only on correctness.

Task 2.5 – Challenge Task

Reviews the equations behind k-means and GMMs.

Compares these theoretical updates with the provided ClusteringFromScratch.ipynb.

Reflects on why the scratch GMM performs worse than scikit-learn’s implementation, particularly the impact of initialisation.

Libraries Used

NumPy – data handling and array operations

Matplotlib – visualisation

scikit-learn – k-means and Gaussian Mixture Models

How to Run

Clone the repository:

git clone <repository-url>


Install required packages:

pip install numpy matplotlib scikit-learn


Open the notebook:

jupyter notebook <student-number>-Clustering.ipynb

Notes

The notebook includes markdown explanations throughout to document the workflow, decisions, and observations when comparing clustering methods. Each task builds on the previous one, moving from data exploration to more flexible probabilistic clustering.
