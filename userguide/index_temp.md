---
title: User Guide
layout: default
---

# {{ page.title }}

<!--
You can use HTML elements in Markdown, such as the comment element, and they won't
be affected by a markdown parser. However, if you create an HTML element in your
markdown file, you cannot use markdown syntax within that element's contents.
-->


<div id="index-grid-full" class="section group">
  <div class="index-paragraph docutils container"><p> <strong> User-guide is under process. For more organized contents, please check <a href="https://spkit.github.io/guide" target="_blank"><font color="DodgerBlue">Example Gallery</font></a> or <a href="https://spkit.readthedocs.io/en/latest/" target="_blank"><font color="DodgerBlue">Documentation</font></a></strong></p></div>
</div>




<div id="index-grid-half" class="section group">
<h2 style="text-align:left;"><u>Getting Started - Table of Content</u></h2>
<h3 style="text-align:left;">
<ul class="simple" style="line-height:1.4;">

<li><a href="https://spkit.readthedocs.io/en/latest/installation.html" target="_blank">Installation</a>
 <ul class="simple"><li><i><font size="3">pip install spkit</font></i></li></ul></li>

 <li><a href="https://spkit.readthedocs.io/en/latest/informationtheory.html#information-theory-for-real-valued-signals" target="_blank">Information Theory</a>
 <h5 style="text-align:left;">
 <ul class="simple">
<li><a href="https://spkit.readthedocs.io/en/latest/informationtheory.html#entropy-of-real-valued-signal" target="_blank">Entropy functions: Shannan, Rényi entropy</a></li>
<li><a href="https://spkit.readthedocs.io/en/latest/informationtheory.html#mutual-information-joint-entropy" target="_blank">Mutual Information & Joint Entropy</a></li>
<li><a href="https://spkit.readthedocs.io/en/latest/informationtheory.html#cross-entropy-kullbackleibler-divergence" target="_blank">Cross Entropy & KL-divergence</a></li>
<li><a href="https://spkit.readthedocs.io/en/latest/informationtheory.html#eeg-signal" target="_blank">EEG Signal Analysis</a></li>
<ul class="simple">
<li><a href="https://spkit.readthedocs.io/en/latest/informationtheory.html#single-channel" target="_blank"><font size="3">Single Channel Analysis</font></a></li>
<li><a href="https://spkit.readthedocs.io/en/latest/informationtheory.html#multi-channels-cross" target="_blank"><font size="3">Multi-channel Analysis, with cross/joint entropy, Mututal Information Wavelet</font></a></li>
 </ul>
<li><a href="https://spkit.readthedocs.io/en/latest/dispersion_entropy.html" target="_blank">Dispersion Entropy</a></li>
 </h5>  
 </ul>
 </li>



  <li><a href="#">Wavelet Analysis</a>
    <h5 style="text-align:left;">
    <ul class="simple">
    <li><a href="https://spkit.readthedocs.io/en/latest/cwt.html" target="_blank">Continues Wavelet Transform - CWT - (complext wavelets)</a></li>
      <ul class="simple">
        <li><a href="https://spkit.readthedocs.io/en/latest/cwt.html#gauss-wavelet" target="_blank"><font size="3">Gauss Wavelet</font></a></li>
        <li><a><font size="3">Morlet Wavelet</font></a></li>
        <li><a><font size="3">Gabor Wavelet</font></a></li>
        <li><a><font size="3">Poisson Wavelet</font></a></li>
        <li><a><font size="3">Maxican Wavelet</font></a></li>
        <li><a><font size="3">Shannan Wavelet</font></a></li>
        </ul>
    <li><a href="https://spkit.github.io/examples/wfilter" target="_blank">Wavelet Filtering</a></li>
    </ul>
    </h5>
  </li>

  <li><a href="#">Signal Decomposition & Synthesis</a>  
    <h5 style="text-align:left;">
    <ul class="simple">
    <li><a href="https://spkit.readthedocs.io/en/latest/analysis_synthesis_models.html#dft-analysis-and-synthesis" target="_blank">Discrete Fourier Transform  - DFT</a></li>
    <li><a href="https://spkit.readthedocs.io/en/latest/analysis_synthesis_models.html#stft-analysis-and-synthesis" target="_blank">Short-Time Fourier Transform - STFT</a></li>
    <li><a href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/FRFT_demo_sine.ipynb" target="_blank">Fractional Fourier Transform</a></li>
    <li><a href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Sinasodal_Model_AnalysisSynthesis.ipynb" target="_blank">Sinasodal Decomposition Model</a></li>
    <li><a href="https://spkit.readthedocs.io/en/latest/ica.html" target="_blank">Independent Component Analysis - ICA</a></li>
    <!--<li><a>Principal Component Analysis, Singular Value Decomposition</a></li>-->
    <li><a href="" target="_blank"></a></li>
    </ul>

  </h5>
  </li>

  <li><a href="https://spkit.github.io/guide/notebooks/Ramanujan_Filter_Banks_for_Period_Estimation_Demo_examples.html">Ramanujan Filter Banks</a>
    <h5 style="text-align:left;">
    <ul class="simple">
    <li><a href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Ramanujan_Filter_Banks_for_Period_Estimation_Demo_examples.ipynb" target="_blank">Ramanujan Filter Banks for period estimation - example 1</a></li>
    <li><a href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Ramanujan_Filter_Banks_for_Period_Estimation_from_signal.ipynb" target="_blank">Ramanujan Filter Banks  - example 2</a></li>
    <li><a href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Ramanujan_Filter_Banks_for_Period_Estimation_with_sparse_penalty.ipynb" target="_blank"></a>Ramanujan Dictionary - with sparse penalty</li>
    <li><a href="" target="_blank"></a></li>
    </ul></li>

  <li><a href="https://spkit.readthedocs.io/en/latest/machinelearning.html" target="_blank">Machine Learning Algorithms</a>
    <h5 style="text-align:left;">
    <ul class="simple">
    <li><a href="https://spkit.readthedocs.io/en/latest/machinelearning.html#naive-bayes" target="_blank">Naive Bayes</a></li>
    <li><a href="https://spkit.readthedocs.io/en/latest/machinelearning.html#logistic-regression" target="_blank">Logistic Regression</a></li>
    <li><a href="https://spkit.readthedocs.io/en/latest/machinelearning.html#decision-trees" target="_blank">Decision Tree</a></li>
    <li><a>Kernel Learning</a></li>
    </ul></li>
  </h5>

  <li><a href="#">Biomedical Signal Processing techniques</a>
    <ul class="simple">
    <li><a href="#">EEG Signals</a>
      <h5 style="text-align:left;">
      <ul class="simple">
      <li><a>Artifact Removal Algorithms</a></li>
        <ul class="simple">
        <li><a href="https://spkit.github.io/guide/notebooks/ATAR_Algorithm_EEG_Artifact_Removal.html" target="_blank">Automatic and Tunable -  ATAR </a></li>
        <li><a href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/ATAR_Algorithm_EEG_Artifact_Removal.ipynb" target="_blank">Automatic and Tunable -  ATAR (jupyter-notebook)</a></li>
        <li><a href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/ICA_based_Artifact_Removal.ipynb" target="_blank">ICA Based</a></li>
        </ul></li>
      <!--<li><a>Wavelet Analysis</a></li>-->
      </ul></li>
      </h5>
      <!--<li><a href="#">GSR</a>
      <ul class="simple">
      <li><a>Phasic and tonic deomposition</a></li>
      <li><a>Wavelet Analysis</a></li>
      </ul>
      </li>-->
    </ul></li>
  x-->

  <li><a href="#">Miscellaneous</a>
    <ul class="simple">
    <li><a href="https://spkit.readthedocs.io/en/latest/pylfsr.html" target="_blank">Linear Feedback Shift Register</a></li>
    </ul></li>
</ul>
</h3>
</div>
<div id="index-grid-full" class="section group"></div>
<div id="index-grid-full" class="section group">
  <div class="index-paragraph docutils container"><p> <strong> For updated version please check <a href="https://spkit.readthedocs.io/en/latest/" target="_blank"><font color="DodgerBlue">documentation</font></a> or  <a href="https://spkit.github.io/guide" target="_blank"><font color="DodgerBlue">New Guide here</font></a></strong></p></div>
</div>