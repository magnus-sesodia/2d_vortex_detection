### **Overview**

This repository contains the models and code used for the paper [CNN-Based vortex detection in atomic 2D Bose gases in the presence of a phononic background](https://iopscience.iop.org/article/10.1088/2632-2153/adbfdc)

**Abstract**

Quantum vortices play a crucial role in both equilibrium and dynamical phenomena in two-dimensional (2D) superfluid systems. Experimental detection of these excitations in 2D ultracold atomic gases typically involves examining density depletions in absorption images, however the presence of a significant phononic background renders the problem challenging, beyond the capability of simple algorithms or the human eye. Here, we utilize a convolutional neural network to detect vortices in the presence of strong long- and intermediate-length scale density modulations in finite-temperature 2D Bose gases. We train the model on datasets obtained from *ab initio* Monte Carlo simulations using the classical-field method for density and phase fluctuations, and Gross–Pitaevskii simulation of realistic expansion dynamics. We use the model to analyze experimental images and benchmark its performance by comparing the results to the matter-wave interferometric detection of vortices, confirming the observed scaling of vortex density across the Berezinskii–Kosterlitz–Thouless critical point. The combination of a relevant simulation pipeline with machine-learning methods is a key development towards the comprehensive understanding of complex vortex-phonon dynamics in out-of-equilibrium 2D quantum systems.

### **Content**

The code is provided in the form of three [Jupyter Notebooks](https://jupyter.org/) written in Python and using the machine-learning libraries [Tensorflow](https://www.tensorflow.org/) & [Keras](https://keras.io/)
There are 3 example notebooks that cover the most important stages of the data pipeline

1. **`preprocessing.ipynb`** - Processing of the simulated data into training data
2. **`training.ipynb`** - Training and validation of the CNN
3. **`inference.ipynb`** - Predicting on experimental images

The trained model used in the paper can be found in **`models/`**

### **Questions**

If you have any questions, feel free to open an issue or [email me](mailto:magnus.sesodia@physics.ox.ac.uk)

### **Citation**

If you use our code/models for your research, consider citing our paper:
```
@article{Sesodia_2025,
  title = {CNN-Based vortex detection in atomic 2D Bose gases in the presence of a phononic background},
  volume = {6},
  ISSN = {2632-2153},
  url = {http://dx.doi.org/10.1088/2632-2153/adbfdc},
  DOI = {10.1088/2632-2153/adbfdc},
  number = {1},
  journal = {Machine Learning: Science and Technology},
  publisher = {IOP Publishing},
  author = {Sesodia,  M and Sunami,  S and Chang,  E and Rydow,  E and Foot,  C J and Beregi,  A},
  year = {2025},
  month = mar,
  pages = {015067}
}
```
