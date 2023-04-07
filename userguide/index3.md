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



Installation
------------

<h2 id="1-install">Installation</h2>

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



1. Filtering
------------

<h3 id="1-1-removing-drift">1.1. Removing Drift</h3>

1.1.1  **[High Pass filter](#1-install)**
1.1.2  **[IIR-1st-order filter](#2-filtering)**
1.1.3  **[Savitzky–Golay filter](#3-informtion-theory)**

<h3 id="1-2-smoothing">1.2. Smoothing</h3>

1.2.1  **[Low Pass filter](#4-wavelet-analysis)**
1.2.2  **[Savitzky–Golay filter](#5-transform-techniques)**
1.2.3  **[Gaussian filter](#6-biomedical)**
1.2.4  **[Mollifier](#7-machine-learning)**

<h3 id="1-install">1.3. Basic filtering</h3>

1.3.1  **[Butter-worth filter LP/HP/BS/BR](#4-wavelet-analysis)**

<h3 id="1-install">1.4. Wavelet Filtering</h3>

1.4.1  **[Wavelet filtering on whole signal](#5-transform-techniques)**
1.4.2  **[Wavelet filtering on smaller windows](#6-biomedical)**
1.4.3  **[Wavelet Packet Analysis filter](#7-machine-learning)**


<h3 id="1-install">1.5. Kernel Filtering</h3>
1.5.1  **[Filtering with Custom kernel](#5-transform-techniques)**

<h3 id="1-install">1.6. Spatial Filter</h3>
1.6.1  **[Proximity based filter](#5-transform-techniques)**
1.6.2  **[Connectivity (Adjuscy Matrix) based filter](#5-transform-techniques)**



<h2 class="no-bg" id="2-filtering">Basic Filtering</h2>














