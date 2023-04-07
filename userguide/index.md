---
title: User Guide
layout: base_ex
---

<div id="index-grid-full" class="section group">
  <div class="index-paragraph docutils container"><p> <strong> Please check <a href="https://spkit.github.io/guide" target="_blank"><font color="DodgerBlue">Example Gallery</font></a> or <a href="https://spkit.readthedocs.io/en/latest/" target="_blank"><font color="DodgerBlue">Documentation</font></a></strong></p></div>
</div>


# Getting started

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


<h2 class="no-bg" id="1-install">Installation</h2>

Installing `spkit` is simple and easy

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

<h2 class="no-bg" id="2-filtering">Basic Filtering</h2>

<h3 class="no-bg" id="">Removing baseline/drift/wander - DC component</h3>


```python
import spkit as sp
Xf = sp.filterDC(X,..)
Xf = sp.filterDC_sGolay(X,..)
Xf = sp.filter_X(X,band =[0.5],btype='highpass',order=5,fs=128.0,ftype='filtfilt')
```

<font size="4"><a href="https://spkit.github.io/docs/docs/filtering.html" target="_blank"> Check here for details</a></font>


<h3 class="no-bg" id="">Filtering</h3>


```python
import spkit as sp

#highpass
Xf = sp.filter_X(X,band =[0.5],btype='highpass',order=5,fs=128.0,ftype='filtfilt')

#bandpass
Xf = sp.filter_X(X,band =[1, 4],btype='bandpass',order=5,fs=128.0,ftype='filtfilt')

#lowpass
Xf = sp.filter_X(X,band =[40],btype='lowpass',order=5,fs=128.0,ftype='filtfilt')
```

<font size="4"><a href="https://spkit.github.io/docs/docs/filtering.html" target="_blank"> Check here for details</a></font>


<h2 class="no-bg" id="3-informtion-theory">Information Theory</h2>
<h2 class="no-bg" id="4-wavelet-analysis">Wavelet Analysis</h2>
<h2 class="no-bg" id="5-transform-techniques">Transform Techniques</h2>
<h2 class="no-bg" id="6-biomedical">Biomedical Signals</h2>
<h2 class="no-bg" id="8-links">Helpful Links</h2>

* [Homepage](http://spkit.github.io) - http://spkit.github.io
* [Documentation](https://spkit.readthedocs.io) - https://spkit.readthedocs.io
* [Documentation in page](http://spkit.github.io/docs) - http://spkit.github.io/docs
* [Example Gallery](http://spkit.github.io/examples) - http://spkit.github.io/examples
* [Github](https://github.com/Nikeshbajaj/spkit) - https://github.com/Nikeshbajaj/spkit
* [PyPi-project](https://pypi.org/project/spkit) - https://pypi.org/project/spkit



<!--
In this section, we explain how to get started with the dataset and modeling. For ease all the necessary element and codes are put into one python library called - ***phyaat***. Here we explain the functionalities that Phyaat library has with possible tuning the process of preprocessing and feature extractions. To start with a quick exmaple to preditive modeling check the [**Predictive Modeling**  ](/modeling) tab.

<font size="4"> For quick start with predictive modeling, check <a href="/modeling/index.html" target="_blank"> <span style="font-weight:bold"> EXAMPLE CODE</span></a></font>
-->
