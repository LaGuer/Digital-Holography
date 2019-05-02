# Digital Holography
Let's play with digital holograms

[![Travis](https://travis-ci.org/LaGuer/Digital-Holography.svg?branch=master)](https://travis-ci.org/LaGuer/Digital-Holography)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LaGuer/Digital-Holography/master)

[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LaGuer/Digital-Holography/blob/master/.ipynb)

<a href="https://notebooks.azure.com/import/gh/LaGuer/Digital-Holography"><img src="https://notebooks.azure.com/launch.png" /></a>

Visualization
-------------

[![nbviewer](https://img.shields.io/badge/view%20on-nbviewer-brightgreen.svg)](https://nbviewer.jupyter.org/github/LaGuer/Digital-Holography/blob/master/.ipynb)

Reference textbook: 

* Digital holography and wavefront sensing by Ulf Schnars, Claas Falldorf, John Watson, and Werner Jüptner, Springer-verlag Berlin an, (2016). (Read section 3.2)

* Introduction to Modern Digital Holography: With Matlab By Ting-Chung Poon, Jung-Ping Liu, Cambridge University Press (2014)

### Digital Hologram
<img src="https://github.com/LaGuer/Digital-Holography/blob/master/ulf7.BMP" width="200" height="200">
'ulf7.BMP' is an *off-axis* digital hologram created by recording an object at about 1 meter distance with HeNe laser (632.8 nm) and an image sensor with 6.8 µm pixel size. The file was kindly provided by Dr. Ulf Schnars.

### 1. Reconstruction by Fresnel approximation
This offers fastest way of reconstructing a hologram (only one FFT operation).
'Fresnel_reconstruction.ipynb' contains the algorithm.  
Fresnel reconstruction result  
<img src="https://github.com/LaGuer/Digital-Holography/blob/master/images/fresnel_reconstruction.png" width="200" height="200">

### 2. Reconstruction by Convolution approach
This offeres most flexible way of reconstructing a hologram. It is possible to numerically adjust the zoom value in the reconstruction. Involves 3 FFT operations. 
'Convolution_reconstruction.ipynb' contains the algorithm.  
Convolution reconstruction result  
<img src="https://github.com/LaGuer/Digital-Holography/blob/master/images/Convolution_reconstruction.png" width="200" height="200">

Convolution reconstruction with suppressed DC term (obtained by using hologram - mean(hologram))  
<img src="https://github.com/LaGuer/Digital-Holography/blob/master/images/Convolution_reconstruction_DCsuppressed.png" width="200" height="200">
