---
title: User Guide
layout: base_ex
---

<div id="index-grid-full" class="section group">
  <div class="index-paragraph docutils container"><p> <strong> Please check <a href="https://spkit.github.io/guide" target="_blank"><font color="DodgerBlue">Example Gallery</font></a> or <a href="https://spkit.readthedocs.io/en/latest/" target="_blank"><font color="DodgerBlue">Documentation</font></a></strong></p></div>
</div>


# User Guide

`spkit` is a python library, aimed to ease the use of signal processing algorithms and techniques. It also includes a few machine learning models with enhanced visulisations.


**Table of Contents**
* **[Installation](#1-install)**
* **[Basic Filtering](#2-filtering)**
* **[Information Theory](#3-informtion-theory)**
* **[Wavelet Analysis](#4-wavelet-analysis)**
* **[Transform Techniques](#5-transform-techniques)**
* **[Biomedical Signals](#6-biomedical)**
* **[Machine Learning](#7-machine-learning)**
* **[Helpful links](#8-links)**



<h1 id="1-install">Installation</h1>

Installing `spkit` is simple ans easy

**with pip**

```console
pip install spkit
```

**with conda -** ***conda-forge is in process***

```console
conda install -c nikeshbajaj spkit
```


**Or build from source**

Download the repository or clone it with git, after cd in directory build it from source with 

```console
python setup.py install
```

<h1 style="background: #97c6d2;" id="1-filtering">1. Filtering</h1>


1\. Filtering
------------

<h2 class="no-bg" id="1-1-removing-drift">1.1. Removing Drift</h2>
* 1.1.1.  **[High Pass filter](#1-install)**
* 1.1.2.  **[IIR-1st-order filter](#2-filtering)**
* 1.1.3.  **[Savitzky–Golay filter](#3-informtion-theory)**

<h2 class="no-bg" id="1-2-smoothing">1.2. Smoothing</h2>
* 1.2.1.  **[Low Pass filter](#4-wavelet-analysis)**
* 1.2.2.  **[Savitzky–Golay filter](#5-transform-techniques)**
* 1.2.3.  **[Gaussian filter](#6-biomedical)**
* 1.2.4.  **[Mollifier](#7-machine-learning)**

<h2 id="1-install">1.3. Basic filtering</h2>
* 1.3.1.  **[Butter-worth filter LP/HP/BS/BR](#4-wavelet-analysis)**

<h2 class="no-bg" id="1-install">1.4. Wavelet Filtering</h2>
* 1.4.1.  **[Wavelet filtering on whole signal](#5-transform-techniques)**
* 1.4.2.  **[Wavelet filtering on smaller windows](#6-biomedical)**
* 1.4.3.  **[Wavelet Packet Analysis filter](#7-machine-learning)**


<h2 class="no-bg" id="1-install">1.5. Kernel Filtering</h2>
* 1.5.1.  **[Filtering with Custom kernel](#5-transform-techniques)**

* <h2 id="1-install">1.6. Spatial Filter</h2>
* 1.6.1.  **[Proximity based filter](#5-transform-techniques)**
* 1.6.2.  **[Connectivity (Adjuscy Matrix) based filter](#5-transform-techniques)**


<!-- # Information Theory -->

<h1 style="background: #97c6d2;" id="2-infomation">2. Information Theory</h1>

2\. Information Theory 
---------------------

<h2 class="no-bg" id="1-1-removing-drift">2.1. Signal as IID Source</h2>

* 2.1.1.  **[Shannan entropy](#1-install)**
* 2.1.2.  **[Rényi entropy](#2-filtering)**
* 2.1.3.  **[Mutual Information](#3-informtion-theory)**
* 2.1.3.  **[Conditional entropy](#3-informtion-theory)**
* 2.1.3.  **[Joint Entropy](#3-informtion-theory)**
* 2.1.3.  **[Cross entropy](#3-informtion-theory)**
* 2.1.3.  **[Kullback–Leibler divergence](#3-informtion-theory)**

<h2 class="no-bg" id="1-1-removing-drift">2.2. Signal as non-IID Source</h2>

* 2.2.1.  **[Approximate Entropy](#1-install)**
* 2.2.2.  **[Sample Entropy](#2-filtering)**
* 2.2.3.  **[Approximate Entropy Vs Sample Entropy](#3-informtion-theory)**
* 2.2.4.  **[Singular Value Decomposition Entropy](#3-informtion-theory)**
* 2.2.5.  **[Spectral Entropy](#3-informtion-theory)**
* 2.2.6.  **[Permutation Entropy](#3-informtion-theory)**
* 2.2.7.  **[Dispersion Entropy](#3-informtion-theory)**

<h2 class="no-bg" id="1-1-removing-drift">2.3. Dispersion Entropy</h2>

* 2.3.1.  **[Dispersion Entropy](#1-install)**
* 2.3.2.  **[Multi-scale Dispersion Entropy](#1-install)**


<h2 class="no-bg" id="1-1-removing-drift">2.4. Differential Entropy ~ Gaussian Distribution</h2>

* 2.1.1  **[Shannan entropy](#1-install)**
* 2.1.2  **[Rényi entropy](#2-filtering)**
* 2.1.3  **[Mutual Information](#3-informtion-theory)**
* 2.1.3  **[Conditional entropy](#3-informtion-theory)**
* 2.1.3  **[Joint Entropy](#3-informtion-theory)**
* 2.1.3  **[Cross entropy](#3-informtion-theory)**
* 2.1.3  **[Kullback–Leibler divergence](#3-informtion-theory)**




<h1 style="background: #97c6d2;" id="3-infomation">3. Ramanujan Filter Bank (RBF)</h1>

<h2 style="background: #97c6d2;" id="3-infomation">3. Ramanujan Filter Bank (RBF)</h2>
* 3.1  **[Period Estimation using RBF](#1-install)**
* 3.2  **[Period Strength Analysis](#2-filtering)**



<h1 style="background: #97c6d2;" id="3-infomation">4. Analysis & Synthesis Models</h1>
<h2 style="background: #97c6d2;" id="3-infomation">4. Analysis & Synthesis Models</h2>

* 4.1  **[Discreet Fourier Transform: Analysis & Synthesis](#1-install)**
* 4.2  **[Short Time Fourier Transform: Analysis & Synthesis](#2-filtering)**
* 4.3  **[Fractional Fourier Transform (FRFT): Analysis & Synthesis](#3-informtion-theory)**
* 4.4  **[Sinasodal Model: Analysis & Synthesis](#3-informtion-theory)**


<h1 style="background: #97c6d2;" id="3-infomation">5. Multi-Electrode-Array (MEA) Processing</h1>


<h1 style="background: #97c6d2;" id="3-infomation">5. Geomatrical Transformations</h1>

<h2 id="3-infomation">5. Geomatrical Transformations</h2>
* 5.1  **[Discreet Fourier Transform: Analysis & Synthesis](#1-install)**
* 5.2  **[Short Time Fourier Transform: Analysis & Synthesis](#2-filtering)**








Entropy of real-valued signal (~ non-IID)
<h2 class="no-bg" id="2-filtering">Basic Filtering</h2>














