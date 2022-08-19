---
title: Gallery - Examples
layout: default1
---

# {{ page.title }}

<script type="text/javascript"
  src="http://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
<script type='text/x-mathjax-config'>
MathJax.Hub.Config({                  
tex2jax: {                  
    inlineMath: [ ['$','$'], ["\[","\]"] ],                  
},                  
"HTML-CSS": {                  
    linebreaks: {                  
        automatic: true                   
    }                  
}                  
});                  
</script>                  
<script type="text/javascript" async src = "https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"></script>

<!--
You can use HTML elements in Markdown, such as the comment element, and they won't
be affected by a markdown parser. However, if you create an HTML element in your
markdown file, you cannot use markdown syntax within that element's contents.
-->
<div id="index-grid-half" class="section group">
<!-- <h1 style="max-width: 90%; text-align:center;background: #F9BE87;display=flex;padding:10px;"><a style="color:black;">Signal Processing Techniques</a></h1> -->
<h1 style="max-width: 80%; text-align:center;background: #F9BE87;"><a style="color:black;">Signal Processing Techniques</a></h1>
  
  

<span id="id2"></span><h1 style="text-align:left;"><a style="color:DodgerBlue;" class="toc-backref" href="#ITC"><span class="section-number"></span>Information Theory based techniques</a></h1>
<p style="text-align:left;"></p>

   <div class="sphx-glr-thumbcontainer" tooltip="Computing entropy of real-valued signal.">
     <div class="figure align-default" id="">
     <img alt="" src="{{"assets/images/entropy_3.jpg" | relative_url }}"/>
     <p class="caption"><span class="caption-text">
     <a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Entropy_example.ipynb"  target="_blank">Entropy of real-valued signal ~ (IID)</a>
     </span>
     </p>
     </div>
   </div>
   <div class="sphx-glr-thumbcontainer" tooltip="Computing entropy of real-valued signal.">
     <div class="figure align-default" id="">
     <img alt="" src="{{"assets/images/entropy_2.jpg" | relative_url }}"/>
     <p class="caption"><span class="caption-text">
     <a class="reference internal" href="https://spkit.readthedocs.io/en/latest/informationtheory.html#entropy-of-real-valued-signal-non-iid"  target="_blank">Entropy of real-valued signal ~ (non-IID)</a></span>
     </p>
     </div>
   </div>
   <div class="sphx-glr-thumbcontainer" tooltip="Multi-channel EEG analysis with Information Theory"><div class="figure align-default" id="id3">
     <img alt="" src="{{"assets/images/EEG_it4.png" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Entropy_EEG_Example.ipynb" target="_blank">Multi-channel EEG signal: Mutual Info, Cross, Joint, Entropy</a></span></p>
     </div>
   </div>
   <div class="sphx-glr-thumbcontainer" tooltip="Venn Diagram and Mutual Info."><div class="figure align-default" id="id3">
     <img alt="" src="{{"assets/images/MutualInfo_Venn_1.gif" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://mybinder.org/v2/gh/Nikeshbajaj/Notebooks/master?urlpath=lab/tree/spkit_SP" target="_blank">Mutual Information and Venn Diagram</a></span>
     </p>
     </div>
   </div>
   <div class="sphx-glr-thumbcontainer" tooltip="Dispersion Entropy"><div class="figure align-default" id="id3">
    <img alt="" src="{{"assets/images/dis_entropy_4.png" | relative_url }}"/>
    <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Dispersion_Entropy_1_demo_EEG.ipynb" target="_blank">Dispersion Entropy</a></span></p>
    </div>
  </div>

<!---================================================================ -->
  <div class="toctree-wrapper compound"></div>
  <hr width="10%">
  <span id="id2"></span><h1 style="text-align:left;"><a style="color:DodgerBlue;" class="toc-backref" href="#wavelet"><span class="section-number"></span>Wavelet Analysis: CWT & DWT</a></h1>
  <p style="text-align:left;"></p>

   <div class="toctree-wrapper compound"></div>
   <div class="sphx-glr-thumbcontainer" tooltip="Scalogram CWT with different wavelets"><div class="figure align-default" id="id3">
     <img alt="" src="{{"assets/images/cwt.jpg" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/ScalogramCWT_v0.0.9.2.ipynb" target="_blank"><span class="std std-ref">Scalogram CWT</span></a></span> </p>
     </div>
   </div>
   <div class="sphx-glr-thumbcontainer" tooltip="Wavelet Filtering"><div class="figure align-default" id="id3">
   <img alt="" src="{{"assets/images/wavelet_filtering_2.png" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="wfilter" target="_blank"><span class="std std-ref">Wavelet Filtering</span></a></span> </p>
   </div>
 </div>
 <div class="sphx-glr-thumbcontainer" tooltip="Automatic and Tunable Artifact Removal Algorithm.">
    <div class="figure align-default" id="">
    <img alt="" src="{{"assets/images/ATAR_Beta_tune_2.gif" | relative_url }}"/>
    <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/ATAR_Algorithm_EEG_Artifact_Removal.ipynb"  target="_blank"><span class="std std-ref">Wavelet based EEG Artifact Removal Algorithm</span></a></span> </p>
    </div>
  </div>


<!---================================================================ -->
 <div class="toctree-wrapper compound"></div>
 <hr width="10%">
 <span id="id2"></span><h1 style="text-align:left;"><a style="color:DodgerBlue;" class="toc-backref" href="#A&S"><span class="section-number"></span>Analysis & Synthesis Models: $f^{-1}(f(x))=\tilde{x}$</a></h1>
 <p style="text-align:left;"></p>
<!--$$f^{-1}(f(x))=\tilde{x}$$-->
 <div class="sphx-glr-thumbcontainer" tooltip="ICA of EEG signal"><div class="figure align-default" id="id3">
   <img alt="" src="{{"assets/images/ICA_EEG_3.jpg" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/ICA_EEG_example.ipynb" target="_blank"><span class="std std-ref">ICA of multi-channel signal</span></a></span> </p>
   </div>
 </div>

 <div class="sphx-glr-thumbcontainer" tooltip="Analysis & Synthesis Models"><div class="figure align-default" id="id3">
    <img alt="" src="{{"assets/images/A&S_blockgiagram_1.png" | relative_url }}"/>
    <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Analysis_Sythesis_Models.ipynb" target="_blank"><span class="std std-ref">Analysis & Synthesis Models: DFT, STFT, FRFT, Sinusodal model</span></a></span> </p>
    </div>
  </div>
  <div class="sphx-glr-thumbcontainer" tooltip="Fractional Fourier Transform"><div class="figure align-default" id="id3">
    <img alt="" src="{{"assets/images/frft_sin_3.gif" | relative_url }}"/>
    <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/FRFT_demo_sine.ipynb" target="_blank"><span class="std std-ref">Fractional Fourier Transform</span></a></span> </p>
    </div>
  </div>

  <div class="sphx-glr-thumbcontainer" tooltip="Sinusodal Model"><div class="figure align-default" id="id3">
    <img alt="" src="{{"assets/images/sinusodal_model_2.png" | relative_url }}"/>
    <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Sinasodal_Model_AnalysisSynthesis.ipynb" target="_blank"><span class="std std-ref">Sinusodal Model for signal decomposion and synthesis</span></a></span> </p>
    </div>
  </div>

<!---================================================================ -->
 <div class="toctree-wrapper compound"></div>
 <hr width="10%">
 <span id="id2"></span><h1 style="text-align:left;"><a style="color:DodgerBlue;" class="toc-backref" href="#A&S"><span class="section-number"></span>Ramanujan Filter bank for periodicity</a></h1>
 <p style="text-align:left;"></p>

   <div class="sphx-glr-thumbcontainer" tooltip="Ramanujan Filter Banks: Demo"><div class="figure align-default" id="id3">
     <img alt="" src="{{"assets/images/RFB_ex2.2.png" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Ramanujan_Filter_Banks_for_Period_Estimation_Demo_examples.ipynb" target="_blank"><span class="std std-ref">Ramanujan Filter Banks: Demo</span></a></span> </p>
     </div>
   </div>

    <div class="sphx-glr-thumbcontainer" tooltip="Ramanujan Filter Banks"><div class="figure align-default" id="id3">
     <img alt="" src="{{"assets/images/RFB_ex1.2.png" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Ramanujan_Filter_Banks_for_Period_Estimation_from_signal.ipynb" target="_blank"><span class="std std-ref">Ramanujan Filter Banks: Signal</span></a></span> </p>
     </div>
   </div>

    <div class="sphx-glr-thumbcontainer" tooltip="Ramanujan Filter Banks with L1 penalty"><div class="figure align-default" id="id3">
     <img alt="" src="{{"assets/images/RFB_l1_ex2.4.png" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/Ramanujan_Filter_Banks_for_Period_Estimation_with_sparse_penalty.ipynb" target="_blank"><span class="std std-ref">Ramanujam Filter Banks: L1 penalty</span></a></span> </p>
     </div>
   </div>

   <div class="sphx-glr-thumbcontainer" tooltip="Binder Links"><div class="figure align-default" id="id3">
     <img alt="" src="https://mybinder.org/badge_logo.svg" height="25em"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://mybinder.org/v2/gh/Nikeshbajaj/Notebooks/master?urlpath=lab/tree/spkit_SP" target="_blank"><span class="std std-ref">In case of broken links, try this</span></a></span> </p>
     </div>
   </div>


<!---================================================================ -->
   <div class="toctree-wrapper compound"></div>
   <hr width="10%">

   <span id="id1"></span><h1 style="text-align:left;"><a style="color:DodgerBlue;" class="toc-backref" href="#EEG"><span class="section-number"></span>EEG Signal Processing & Artifact Removal Algorithms</a>
   <a class="headerlink" href="#eeg" title="Permalink to this headline">¶</a></h1>
   <p style="text-align:left;"></p>

  <div class="sphx-glr-thumbcontainer" tooltip="Automatic and Tunable Artifact Removal Algorithm.">
     <div class="figure align-default" id="">
     <img alt="" src="{{"assets/images/ATAR_Beta_tune_2.gif" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/ATAR_Algorithm_EEG_Artifact_Removal.ipynb"  target="_blank"><span class="std std-ref">ATAR Algorithm</span></a></span> </p>
     </div>
   </div>
  <div class="sphx-glr-thumbcontainer" tooltip="ICA based Artifact Removal Algorithm.">
     <div class="figure align-default" id="">
     <img alt="" src="{{"assets/images/ICA_Artifact_Removal.png" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/SP/ICA_based_Artifact_Removal.ipynb"  target="_blank"><span class="std std-ref">ICA based Algorithm</span></a></span> </p>
     </div>
   </div>
   <div class="sphx-glr-thumbcontainer" tooltip="Topographical Maps.">
      <div class="figure align-default" id="">
      <img alt="" src="{{"examples/figures/eeg_dynamic_ssfi_1.gif" | relative_url }}"/>
      <p class="caption"><span class="caption-text"><a class="reference internal" href="gen_topo"  target="_blank"><span class="std std-ref">Topographic Map</span></a></span> </p>
      </div>
    </div>


   <div class="toctree-wrapper compound"></div>
   <hr width="10%">
   <h4 style="text-align:left;">Click here to try examples: <a class="reference external" href="https://mybinder.org/v2/gh/Nikeshbajaj/Notebooks/master?urlpath=lab/tree/spkit_SP" target="_blank"><img src="https://mybinder.org/badge_logo.svg" height="25em"></a> </h4>
 </div>
 <div class="toctree-wrapper compound"></div>

<!--
<div id="index-grid-half" class="section group">
   <span id="id1"></span><h1 style="text-align:left;"><a style="color:DodgerBlue;" class="toc-backref" href="#EEG"><span class="section-number"></span>EEG Signal Processing</a>
   <a class="headerlink" href="#artifact-eeg" title="Permalink to this headline">¶</a></h1>
   <p style="text-align:left;"></p>
  <div class="sphx-glr-thumbcontainer" tooltip="Topographical Maps.">
     <div class="figure align-default" id="">
     <img alt="" src="{{"examples/figures/eeg_dynamic_ssfi_1.gif" | relative_url }}"/>
     <p class="caption"><span class="caption-text"><a class="reference internal" href="gen_topo"  target="_blank"><span class="std std-ref">Topographic Map</span></a></span> </p>
     </div>
   </div>
   <div class="toctree-wrapper compound"></div>
   <hr width="10%">
  </div> -->



 <div id="index-grid-half" class="section group">
<!--<h1 style="text-align:center; background: #F9BE87;"><a style="color:black;" class="toc-backref" href="#ML">Machine Learning Models with visualization</a></h1>-->
<h1 style="max-width: 80%; text-align:center; background: #F9BE87;"><a style="color:black;" class="toc-backref" href="#ML">Machine Learning Models with visualization</a><a class="headerlink" href="#ML" title="Permalink to this headline">¶</a></h1>

 <span id="id1"></span><h1 style="text-align:left;"><a style="color:DodgerBlue;" class="toc-backref" href="#LR"><span class="section-number"></span>Logistic Regression & Naïve Bayes</a></h1>
 <p style="text-align:left;">Examples of Logistic Regression with SpKit</p>
 <div class="sphx-glr-thumbcontainer" tooltip="An example to demonstrate the visulization of Logistic Regression while training and plotting resulting weights.">
   <div class="figure align-default" id="">
   <img alt="" src="{{"assets/images/LR_v1.gif" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.jupyter.org/github/Nikeshbajaj/Notebooks/blob/master/spkit_ML/LogisticRegression/1_LogisticRegression_examples_spkit.ipynb"  target="_blank"><span class="std std-ref">Logistic Regression</span></a></span> </p>
   </div>
 </div>

 <div class="toctree-wrapper compound"></div>

 <div class="sphx-glr-thumbcontainer" tooltip="Analysing weights"><div class="figure align-default" id="id3">
   <img alt="" src="{{"assets/images/LR_v2.png" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.jupyter.org/github/Nikeshbajaj/Notebooks/blob/master/spkit_ML/LogisticRegression/2_LogisticRegression_Examples_spkitV0.0.9.ipynb" target="_blank"><span class="std std-ref">Logistic Regression for MultiClass</span></a></span> </p>
   </div>
 </div>

 <div class="sphx-glr-thumbcontainer" tooltip="Naive Bayes"><div class="figure align-default" id="id3">
   <img alt="" src="{{"assets/images/Bayes_rule.png" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.jupyter.org/github/Nikeshbajaj/Notebooks/blob/master/spkit_ML/NaiveBayes/1_NaiveBayes_example_spkit.ipynb"><span class="std std-ref">Naïve Bayes</span></a></span> </p>
   </div>
 </div>

 <div class="sphx-glr-thumbcontainer" tooltip="Analysing weights"><div class="figure align-default" id="id3">
   <img alt="" src="{{"assets/images/NaiveBayes_1.png" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.jupyter.org/github/Nikeshbajaj/Notebooks/blob/master/spkit_ML/NaiveBayes/1_NaiveBayes_example_spkit.ipynb" target="_blank"><span class="std std-ref">Naïve Bayes for MultiClass</span></a></span> </p>
   </div>
 </div>


 <div class="toctree-wrapper compound"></div>
 <hr width="10%">
 <h4 style="text-align:left;">Click here to try examples on cloud LR: <a class="reference external" href="https://mybinder.org/v2/gh/Nikeshbajaj/Notebooks/master?urlpath=lab/tree/spkit_ML/LogisticRegression" target="_blank"><img src="https://mybinder.org/badge_logo.svg" height="25em"></a> NB: <a class="reference external" href="https://mybinder.org/v2/gh/Nikeshbajaj/Notebooks/master?urlpath=lab/tree/spkit_ML/NaiveBayes"><img src="https://mybinder.org/badge_logo.svg" height="25em"></a></h4>
 </div>

 <div id="index-grid-half" class="section group">
 <span id="id1"></span><h1 style="text-align:left;"><a style="color:DodgerBlue;" class="toc-backref" href="#trees"><span class="section-number"></span>Decision Trees</a></h1>
 <p style="text-align:left;">Examples of Decision Tree with SpKit</p>

 <div class="sphx-glr-thumbcontainer" tooltip="An example to demonstrate the visulization of tree while training and plotting resulting tree.">
   <div class="figure align-default" id="">
   <img alt="" src="{{"assets/images/tree-viz.gif" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.jupyter.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/0.0.9/ML/Trees/1_DecisionTree_Visualization_spkit_v0.0.9.ipynb" target="_blank"><span class="std std-ref">Decision Tree with Visulization</span></a></span> </p>
   </div>
 </div>

 <div class="toctree-wrapper compound"></div>

 <div class="sphx-glr-thumbcontainer" tooltip="Analysing depth and decision boundries"><div class="figure align-default" id="id3">
   <img alt="" src="{{"assets/images/trees-grid.png" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.jupyter.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/0.0.9/ML/Trees/2_ClassificationTrees_Depth_DecisionBoundaries_spkit_v0.0.9.ipynb" target="_blank"><span class="std std-ref">Effect of Depth on Decision Boundry</span></a></span> </p>
   </div>
 </div>

 <div class="toctree-wrapper compound"></div>

 <div class="sphx-glr-thumbcontainer" tooltip="AN example to show the shrinking capability of tree from SpKit"><div class="figure align-default" id="id4">
   <img alt="" src="{{"assets/images/tree-shrink.png" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.jupyter.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/0.0.9/ML/Trees/3_DecisionTrees_ShrinkingCapability_spkit_v0.0.9.ipynb" target="_blank"><span class="std std-ref">Shrinking Capability of Tree with SpKit</span></a></span></p>
   </div>
 </div>

 <div class="toctree-wrapper compound"></div>

 <div class="sphx-glr-thumbcontainer" tooltip="An example showing how to use catogorical features without need of any enconding"><div class="figure align-default" id="id5">
   <img alt="" src="{{"assets/images/tree-cat.png" | relative_url }}"/>
   <p class="caption"><span class="caption-text"><a class="reference internal" href="https://nbviewer.jupyter.org/github/Nikeshbajaj/Notebooks/blob/master/spkit/0.0.9/ML/Trees/4_DecisionTrees_CatogoricalFeatures_spkit_v0.0.9.ipynb" target="_blank"><span class="std std-ref">Use of Catogorical Features without encoding</span></a></span></p>
   </div>
 </div>
 <div class="toctree-wrapper compound"></div>
 <hr width="10%">
 <h4 style="text-align:left;">Click here to try examples on cloud <a class="reference external" href="https://mybinder.org/v2/gh/Nikeshbajaj/Notebooks/master?urlpath=lab/tree/spkit/0.0.9/ML/Trees" target="_blank"><img src="https://mybinder.org/badge_logo.svg" height="20em"></a>
 </h4>
 </div>


 <div id="index-grid-half" class="section group">
 <span id="id1"></span><h1 style="text-align:left;"><a style="color:blue;" class="toc-backref" href="#logit"><span class="section-number"></span>..</a>
   <hr width="10%">
   <!--<h3 style="text-align:left;">More to come ..</h3> -->

 <!--</div>-->
<!--
 <div id="index-grid-half" class="section group">
 <span id="id1"></span><h1 style="text-align:left;"><a style="color:blue;" class="toc-backref" href="#RF"><span class="section-number"></span>Random Forest</a>
 <a class="headerlink" href="#tutorial-examples" title="Permalink to this headline">¶</a></h1>
 <p style="text-align:left;">Examples with SpKit</p>
 </div>
-->

<!--
 <div id="index-grid-half" class="section group">
 <span id="id1"></span><h1 style="text-align:left;"><a style="color:blue;" class="toc-backref" href="#SVM"><span class="section-number"></span>Spport Vector Machine</a>
 <a class="headerlink" href="#tutorial-examples" title="Permalink to this headline">¶</a></h1>
 <p style="text-align:left;">Examples with SpKit</p>
 </div>
-->
<!--
 <div id="index-grid-half" class="section group">
 <span id="id1"></span><h1 style="text-align:left;"><a style="color:blue;" class="toc-backref" href="#NN"><span class="section-number"></span>Neural Networks</a>
 <a class="headerlink" href="#tutorial-examples" title="Permalink to this headline">¶</a></h1>
 <p style="text-align:left;">Examples with SpKit</p>
 </div>
-->
<!--
 <div id="index-grid-half" class="section group">
 <span id="id1"></span><h1 style="text-align:left;"><a style="color:blue;" class="toc-backref" href="#ensemble"><span class="section-number"></span>Ensemble Approach</a>
 <a class="headerlink" href="#tutorial-examples" title="Permalink to this headline">¶</a></h1>
 <p style="text-align:left;">Examples with SpKit</p>
 </div>
-->
 <!-- </div> -->


<!--
 <div id="index-grid-full" class="section group"></div>
 <div id="getting-started"><a href="{{"userguide" | relative_url }}" class="btn btn-primary">Getting Started</a></div>
 <div id="index-grid-full" class="section group"></div>
-->