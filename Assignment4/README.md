# Applied Data Science 2026 - Assignment 4

## Overview

This repository contains my notebooks for Assignment 4 of the Applied Data Science course.

The main goal of this assignment is to practice modern data science workflows.
The notebooks include machine learning pipelines, imbalanced data methods, generative models, and explainable AI.

Main topics:

* ML Pipelines
* Imbalanced Data
* Variational Autoencoder
* Generative Adversarial Network
* Diffusion Model
* Explainable AI
* End-to-End Workflow

---

## Repository Structure

```text id="2deopp"
Assignment4/
│
├── Assignment4_Part1_ML_Pipelines.ipynb
├── Assignment4_Part2_Imbalanced_Data.ipynb
├── Assignment4_Part3_VAE_FashionMNIST.ipynb
├── Assignment4_Part4_GAN_MNIST.ipynb
├── Assignment4_Part5_DDPM_MNIST.ipynb
├── Assignment4_Part6_XAI_CNN.ipynb
├── Assignment4_Optional_Bonus_End_to_End_Workflow.ipynb
│
├── data/
│   ├── classification_DATA.csv
│   └── Data.csv
│
└── README.md
```

---

## Part 1 - ML Pipelines

File:

```text id="l24h92"
Assignment4_Part1_ML_Pipelines.ipynb
```

This notebook builds a complete machine learning pipeline.

Main work:

* Data loading and basic checking
* Data cleaning with `pandas.pipe`
* Custom validation functions
* Scikit-learn preprocessing pipeline
* Feature scaling
* Categorical encoding
* Missing value handling
* Comparison of different imputers
* Final classifier pipeline
* Saving and loading the full pipeline

Main idea:

A pipeline makes the workflow cleaner, safer, and easier to reuse.

---

## Part 2 - Imbalanced Data

File:

```text id="cxkwbi"
Assignment4_Part2_Imbalanced_Data.ipynb
```

This notebook studies an imbalanced classification problem.

Main work:

* Checking class imbalance
* Random undersampling
* Random oversampling
* SMOTE
* Cost-sensitive learning
* Class weights
* Model comparison with suitable metrics

Main metrics:

* Accuracy
* Balanced Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC
* PR-AUC

Main idea:

For imbalanced data, accuracy can be misleading.
Recall, F1-score, and PR-AUC give more useful information about the minority class.

---

## Part 3 - VAE on Fashion-MNIST

File:

```text id="0efg6p"
Assignment4_Part3_VAE_FashionMNIST.ipynb
```

This notebook implements a Variational Autoencoder.

Dataset:

```text id="nh1pwc"
Fashion-MNIST
```

Main work:

* Encoder network
* Decoder network
* Reparameterization trick
* Reconstruction loss
* KL-divergence loss
* Beta-VAE experiment
* Latent space visualization
* Image reconstruction
* New image generation
* Latent interpolation

Main idea:

The VAE learns a latent space.
Changing beta changes the balance between image quality and latent regularization.

---

## Part 4 - GAN on MNIST

File:

```text id="3w3t4e"
Assignment4_Part4_GAN_MNIST.ipynb
```

This notebook implements a simple GAN.

Dataset:

```text id="m5o775"
MNIST
```

Main work:

* Generator model
* Discriminator model
* Adversarial training loop
* Binary cross-entropy loss
* Generated images during training
* Generator and discriminator loss plots
* Mode collapse discussion

Main idea:

GANs can generate realistic samples, but training can be unstable.
Mode collapse is one possible problem, but it is not guaranteed to happen.

---

## Part 5 - DDPM on MNIST

File:

```text id="cl7sgq"
Assignment4_Part5_DDPM_MNIST.ipynb
```

This notebook implements a simple denoising diffusion model.

Dataset:

```text id="wj69sw"
MNIST
```

Main work:

* Forward noising process
* Denoising model
* Noise prediction objective
* Timestep embedding
* Linear noise schedule
* Cosine noise schedule
* Generated samples
* Comparison between DDPM and GAN

Main idea:

Diffusion models are usually more stable than GANs.
They can also generate diverse samples, but they need more training time.

---

## Part 6 - Explainable AI

File:

```text id="v4bdus"
Assignment4_Part6_XAI_CNN.ipynb
```

This notebook explains the behavior of a CNN model.

Dataset:

```text id="h2fesz"
CIFAR-10
```

Main work:

* CNN model analysis
* Correct prediction examples
* Misclassified image examples
* Grad-CAM heatmaps
* SHAP explanations
* LIME superpixel explanations
* ELI5-style feature importance
* Analysis of wrong predictions

Main idea:

XAI methods help us understand what the model is looking at.
They are useful, but they are not perfect proof of model reasoning.

---

## Optional Bonus - End-to-End Workflow

File:

```text id="iqbbjv"
Assignment4_Optional_Bonus_End_to_End_Workflow.ipynb
```

This notebook combines the main parts of the assignment into one workflow.

Workflow:

```text id="3y1fzb"
Data Cleaning → ML Pipeline → Imbalance Handling → Generative Model → XAI
```

Main work:

* Cleaning a tabular dataset
* Building a machine learning pipeline
* Applying imbalance handling methods
* Using a tabular generative model
* Explaining the final model with XAI
* Comparing results before and after each stage

Main idea:

A full data science workflow is not only about model training.
It also needs cleaning, evaluation, interpretation, and trade-off analysis.

---

## Datasets

This assignment uses tabular and image datasets.

Tabular datasets:

* Loan classification dataset
* Real estate dataset

Image datasets:

* MNIST
* Fashion-MNIST
* CIFAR-10

---

## Main Libraries

The main libraries used in this assignment are:

```text id="tlf6fo"
numpy
pandas
matplotlib
seaborn
scikit-learn
imbalanced-learn
tensorflow
shap
lime
eli5
joblib
```

---

## Notes

* The notebooks are written in a clear and modular way.
* Each important step has a short explanation.
* Some deep learning models use small training settings to save time.
* The focus is on understanding the workflow, not only on high accuracy.
* The final results include tables, plots, generated images, and explanations.

---

## Final Summary

This assignment shows different parts of a modern machine learning workflow.

Main lessons:

* Pipelines make ML projects easier to manage.
* Imbalanced data needs careful evaluation.
* VAEs learn latent spaces and generate new samples.
* GANs can generate images but may be unstable.
* DDPMs are stable but slower to train.
* XAI helps explain model behavior.
* End-to-end workflows need both modeling and interpretation.
