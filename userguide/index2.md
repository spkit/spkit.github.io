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

| Syntax | Description |
| --- | ----------- |
| ```filterDC(X, alpha=256,)``` 		| Text |
| ```filterDC_sGolay(X, window_length=127, polyorder=3)``` 		| Text |
| ```filter_X(X, fs=128.0, band=[0.5], btype='highpass', ftype='filtfilt')``` 		| Text |
| ```filter_powerline(X, fs=1000, powerline=50)``` 		| Text |
| ```filter_smooth_gauss(X, window_length=11)``` 		| Text |
| ```filter_smooth_mollifier(X, window_length=11)``` 		| Text |
| ```filter_smooth_sGolay(X, window_length=127, polyorder=3)``` 		| Text |
| ```filter_with_kernel(X, kernel, iterations=1)``` 		| Text |
| ```filtering_pipeline(X, fs, trim=[0, 0], iir_alpha=0, sg_window=1001, sg_polyorder=1, sg_itr=1, filter_lpf=None, filter_pwrline=None)``` 		| Text |
| ```spatial_filter_adj(X, AdjM, ftype='mean')``` 		| Text |
| ```spatial_filter_dist(X, V, r=0.1, ftype='mean')``` 		| Text |
| ```wavelet_filtering(x, wv='db3', threshold='optimal', wpd_maxlevel=None)``` 		| Text |
| ```wavelet_filtering_win(x, winsize=128, wv='db3', threshold='optimal', filter_out_below=True)``` 		| Text |




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

<style>
table {
    border-collapse: collapse;
}
table, th, td {
   border: 1px solid black;
}
blockquote {
    border-left: solid blue;
    padding-left: 10px;
}
</style>


| Syntax | Description |
| --- | ----------- |
|```entropy(x)```		              | Text |
|```entropy_cond(x)```		| Text |
|```entropy_cross(x)```		| Text |
|```entropy_joint(x)```		| Text |
|```mutual_Info(x, y)```	| Text |
|```entropy_kld(x)```		  | Text |
|```entropy_approx(X, m, r)```		| Text |
|```entropy_sample(X, m, r)```	| Text |
|```entropy_spectral(x)```		  | Text |
|```entropy_svd(x)```		        | Text |
|```entropy_permutation(x)```		| Text |



|] Syntax |] Description ]|
| --- | ----------- |
|] ```entropy_differential(x)```	|] Text ]|
|] ```entropy_diff_cond(X)```		  |] Text ]|
|] ```entropy_diff_cond_self(X)```|] Text ]|
|] ```entropy_diff_joint(x, y)```	|] Text ]|
|] ```entropy_diff_joint_cond(X)```|] Text ]|
|] ```mutual_info_diff_self(X)```|] Text ]|
|] ```mutual_info_diff(X, Y)```|] Text ]|
|] ```transfer_entropy(X, Y)```|] Text ]|
|] ```transfer_entropy_cond(X, Y, Z)```|] Text ]|
|] ```partial_transfer_entropy(X, Y, Z)```|] Text ]|
|] ```entropy_granger_causality(X)```|] Text ]|




Entropy Functions:
~~~~~~~~~

.. list-table:: **Clocking (running LFSR)**
   :widths: 30 50
   :header-rows: 1

   * - Method
     - Discription
   * - ``entropy(x)``
     - Executing/running one cycle
   * - ``entropy(x)``
     - Executing/running k cycles
   * - ``entropy(x)``
     - Executing/running a full period of cylces



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
