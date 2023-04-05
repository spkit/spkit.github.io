---
title: User Guide
layout: base_ex
---
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
  | ```filtering_pipeline(X, fs,...)``` 		| Text |
  | ```spatial_filter_adj(X, AdjM, ftype='mean')``` 		| Text |
  | ```spatial_filter_dist(X, V, r=0.1, ftype='mean')``` 		| Text |



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

<h3 class="no-bg">Differential Entropy</h3>

| Syntax | Description |
| --- | ----------- |
| ```entropy_differential(x)```	| Text |
| ```entropy_diff_cond(X)```		  | Text |
| ```entropy_diff_cond_self(X)```| Text |
| ```entropy_diff_joint(x, y)```	| Text |
| ```entropy_diff_joint_cond(X)```| Text |
| ```mutual_info_diff_self(X)```| Text |
| ```mutual_info_diff(X, Y)```| Text |
| ```transfer_entropy(X, Y)```| Text |
| ```transfer_entropy_cond(X, Y, Z)```| Text |
| ```partial_transfer_entropy(X, Y, Z)```| Text |
| ```entropy_granger_causality(X)```| Text |




<h2 class="no-bg">Core Module</h2>

| Syntax | Description |
| --- | ----------- |
| ```A_law(x,...)``` 		| Text |
| ```Create_Dictionary(Nmax,...)``` 		| Text |
| ```HistPlot(x,...)``` 		| Text |
| ```Mu_law(x,...)``` 		| Text |
| ```OutLiers(x,...)``` 		| Text |
| ```PeriodStrength(x,...)``` 		| Text |
| ```Periodogram(x,...)``` 		| Text |
| ```RFB(x,...)``` 		| Text |
| ```RFB_example_1(period=10,...)``` 		| Text |
| ```RFB_example_2(periods=[3,...)``` 		| Text |
| ```RFB_prange(x,...)``` 		| Text |
| ```SVD(X,...)``` 		| Text |
| ```TD_Embed(x,...)``` 		| Text |
| ```TWM_algo(pfreq,...)``` 		| Text |
| ```WPA_coeff(x,...)``` 		| Text |
| ```WPA_plot(x,...)``` 		| Text |
| ```WPA_temporal(x,...)``` 		| Text |
| ```add_noise(x,...)``` 		| Text |
| ```agg_angles(thetas,...)``` 		| Text |
| ```amplitude_equalizer(x,...)``` 		| Text |
| ```binSize_FD(x)``` 		| Text |
| ```bin_width(x,...)``` 		| Text |
| ```blackman_lobe(x,...)``` 		| Text |
| ```cdf_mapping(x)``` 		| Text |
| ```clean_phase(xp,...)``` 		| Text |
| ```conv1d_fb(x,...)``` 		| Text |
| ```conv1d_fft(x,...)``` 		| Text |
| ```conv1d_nan(x,...)``` 		| Text |
| ```conv2d_nan(x,...)``` 		| Text |
| ```create_multidim_space_signal(x,...)``` 		| Text |
| ```create_signal_1d(n=100,...)``` 		| Text |
| ```create_signal_2d(n=100,...)``` 		| Text |
| ```denorm_kernel(kernel,...)``` 		| Text |
| ```dft_analysis(x,...)``` 		| Text |
| ```dft_synthesis(mX,...)``` 		| Text |
| ```direction_flow_map(X_theta,...)``` 		| Text |
| ```dispersion_entropy(x,...)``` 		| Text |
| ```dispersion_entropy_multiscale_refined(x,...)``` 		| Text |
| ```dominent_freq(X,...)``` 		| Text |
| ```dominent_freq_win(X,...)``` 		| Text |
| ```entropy(x,...)``` 		| Text |
| ```entropy_approx(X,...)``` 		| Text |
| ```entropy_cond(x,...)``` 		| Text |
| ```entropy_cross(x,...)``` 		| Text |
| ```entropy_diff_cond(X,...)``` 		| Text |
| ```entropy_diff_cond_self(X,...)``` 		| Text |
| ```entropy_diff_joint(x,...)``` 		| Text |
| ```entropy_diff_joint_cond(X,...)``` 		| Text |
| ```entropy_differential(x,...)``` 		| Text |
| ```entropy_granger_causality(X,...)``` 		| Text |
| ```entropy_joint(x,...)``` 		| Text |
| ```entropy_kld(x,...)``` 		| Text |
| ```entropy_permutation(x,...)``` 		| Text |
| ```entropy_sample(X,...)``` 		| Text |
| ```entropy_spectral(x,...)``` 		| Text |
| ```entropy_svd(x,...)``` 		| Text |
| ```f0_detection(x,...)``` 		| Text |
| ```ffrft(x,...)``` 		| Text |
| ```fill_nans_1d(x,...)``` 		| Text |
| ```fill_nans_2d(X,...)``` 		| Text |
| ```filterDC(X,...)``` 		| Text |
| ```filterDC_X(X,...)``` 		| Text |
| ```filterDC_sGolay(X,...)``` 		| Text |
| ```filter_X(X,...)``` 		| Text |
| ```filter_powerline(X,...)``` 		| Text |
| ```filter_smooth_gauss(X,...)``` 		| Text |
| ```filter_smooth_mollifier(X,...)``` 		| Text |
| ```filter_smooth_sGolay(X,...)``` 		| Text |
| ```filter_with_kernel(X,...)``` 		| Text |
| ```filtering_pipeline(X,...)``` 		| Text |
| ```frft(x,...)``` 		| Text |
| ```friedrichs_mollifier_kernel(window_size,...)``` 		| Text |
| ```gaussian_kernel(window_length,...)``` 		| Text |
| ```getQuickStats(x)``` 		| Text |
| ```getStats(x,...)``` 		| Text |
| ```get_activation_time(x,...)``` 		| Text |
| ```get_repolarisation_time(x,...)``` 		| Text |
| ```iffrft(x,...)``` 		| Text |
| ```ifrft(x,...)``` 		| Text |
| ```infomax(data,...)``` 		| Text |
| ```isPower2(n)``` 		| Text |
| ```low_resolution(x,...)``` 		| Text |
| ```mean_minSE(x,...)``` 		| Text |
| ```minMSE(x,...)``` 		| Text |
| ```mutual_Info(x,...)``` 		| Text |
| ```mutual_info_diff(X,...)``` 		| Text |
| ```mutual_info_diff_self(X,...)``` 		| Text |
| ```partial_transfer_entropy(X,...)``` 		| Text |
| ```partial_transfer_entropy_(X,...)``` 		| Text |
| ```peak_detection(mX,...)``` 		| Text |
| ```peak_interp(mX,...)``` 		| Text |
| ```phase_map(X,...)``` 		| Text |
| ```phase_map_reconstruction(X,...)``` 		| Text |
| ```plotJointEntropyXY(x,...)``` 		| Text |
| ```quantize_FD(x,...)``` 		| Text |
| ```quantize_signal(x,...)``` 		| Text |
| ```show_compass(Ax_theta,...)``` 		| Text |
| ```show_farmulas()``` 		| Text |
| ```signal_delayed_space(x,...)``` 		| Text |
| ```signal_diff(x,...)``` 		| Text |
| ```signal_embeddings(x,...)``` 		| Text |
| ```simplify_signal(x,...)``` 		| Text |
| ```sinc_dirichlet(x,...)``` 		| Text |
| ```sinc_interp(x)``` 		| Text |
| ```sineModel_analysis(x,...)``` 		| Text |
| ```sineModel_synthesis(fXt,...)``` 		| Text |
| ```sine_spectrum(ipfreq,...)``` 		| Text |
| ```sinetracks_cleaning(tfreq,...)``` 		| Text |
| ```spatial_filter_adj(X,...)``` 		| Text |
| ```spatial_filter_dist(X,...)``` 		| Text |
| ```stft_analysis(x,...)``` 		| Text |
| ```stft_synthesis(mXt,...)``` 		| Text |
| ```transfer_entropy(X,...)``` 		| Text |
| ```transfer_entropy_cond(X,...)``` 		| Text |
| ```wavelet_filtering(x,...)``` 		| Text |
| ```wavelet_filtering_win(x,...)``` 		| Text |



<h2 class="no-bg" id="4-wavelet-analysis">Wavelet Analysis</h2>

    | Syntax | Description |
    | --- | ----------- |
    | ```wavelet_filtering(x, wv='db3', threshold='optimal',...)``` 		| Text |
    | ```wavelet_filtering_win(x, winsize=128, ..)``` 		| Text |

<h2 class="no-bg" id="5-transform-techniques">Transform Techniques</h2>
<h2 class="no-bg" id="6-biomedical">Biomedical Signals</h2>



<h2 class="no-bg">EEG Module</h2>


| Syntax | Description |
| --- | ----------- |
| ```eeg.ATAR(X,...)``` 		| Text |
| ```eeg.ATAR_1Ch(x,...)``` 		| Text |
| ```eeg.ATAR_mCh(X,...)``` 		| Text |
| ```eeg.ATAR_mCh_noParallel(X,...)``` 		| Text |
| ```eeg.CBIeye(Wnr,...)``` 		| Text |
| ```eeg.Elimination(w,...)``` 		| Text |
| ```eeg.Gen_SSFI(X,...)``` 		| Text |
| ```eeg.GridInterpolation(pos,...)``` 		| Text |
| ```eeg.ICA_filtering(X,...)``` 		| Text |
| ```eeg.ICAremoveArtifact(x,...)``` 		| Text |
| ```eeg.LinearAttenuanating(w,...)``` 		| Text |
| ```eeg.Periodogram(x,...)``` 		| Text |
| ```eeg.RhythmicDecomposition(E,...)``` 		| Text |
| ```eeg.SoftThresholding(w,...)``` 		| Text |
| ```eeg.TopoMap(pos,...)``` 		| Text |
| ```eeg.Wfilter(x,...)``` 		| Text |
| ```eeg.s1020_get_epos2d_(ch_names,...)``` 		| Text |
| ```eeg.showTOPO(Zi,...)``` 		| Text |


<h2 class="no-bg">MEA Module</h2>


| Syntax | Description |
| --- | ----------- |
| ```mea.activation_repol_time_loc(X,...)``` 		| Text |
| ```mea.activation_time_loc(X,...)``` 		| Text |
| ```mea.align_cycles(X,...)``` 		| Text |
| ```mea.analyse_mea_file(file_name,...)``` 		| Text |
| ```mea.arrange_mea_grid(features,...)``` 		| Text |
| ```mea.ch_idx2label(ch_idx,...)``` 		| Text |
| ```mea.ch_label2idx(ch_list,...)``` 		| Text |
| ```mea.channel_mask(mask_ch,...)``` 		| Text |
| ```mea.compute_cv(Ax,...)``` 		| Text |
| ```mea.egm_features(x,...)``` 		| Text |
| ```mea.extract_egm(X,...)``` 		| Text |
| ```mea.feature_mat(features,...)``` 		| Text |
| ```mea.find_bad_channels_idx(X,...)``` 		| Text |
| ```mea.get_stim_loc(X,...)``` 		| Text |
| ```mea.mat_1_show(A,...)``` 		| Text |
| ```mea.mat_list_show(A,...)``` 		| Text |
| ```mea.mea_feature_map(features,...)``` 		| Text |
| ```mea.plot_mea_grid(X,...)``` 		| Text |
| ```mea.unarrange_mea_grid(M,...)``` 		| Text |


<h2 class="no-bg">Stats Module</h2>

| Syntax | Description |
| --- | ----------- |
| ```stats._getSS(p,...)``` 		| Text |
| ```stats.entropy(x,...)``` 		| Text |
| ```stats.f_oneway(*samples,...)``` 		| Text |
| ```stats.get_stats(x,...)``` 		| Text |
| ```stats.outliers(x,...)``` 		| Text |
| ```stats.plotBoxes_groups(xi,...)``` 		| Text |
| ```stats.quick_stats(x,...)``` 		| Text |
| ```stats.test_2groups(x1,...)``` 		| Text |
| ```stats.test_groups(x,...)``` 		| Text |


<h2 class="no-bg">IO Module</h2>


| Syntax | Description |
| --- | ----------- |
| ```io.read_bdf(file_name,...)``` 		| Text |
| ```io.read_hdf(file_name,...)``` 		| Text |
| ```io.read_surf_file(file_name)``` 		| Text |
| ```io.view_hierarchical_order(file_obj,...)``` 		| Text |
| ```io.write_vtk(filename,...)``` 		| Text |


<h2 class="no-bg">Geometry Module</h2>



| Syntax | Description |
| --- | ----------- |
| ```geometry.Elliptical(X,...)``` 		| Text |
| ```geometry.FGSquircular(X,...)``` 		| Text |
| ```geometry.RadialMapping(X,...)``` 		| Text |
| ```geometry.SchwarzChristoffel(X,...)``` 		| Text |
| ```geometry.ShirleyEA(X,...)``` 		| Text |
| ```geometry.area_tri(p1,...)``` 		| Text |
| ```geometry.car2spar(X)``` 		| Text |
| ```geometry.create_random_map_2d(n_samples=500,...)``` 		| Text |
| ```geometry.create_signal_1d(n=100,...)``` 		| Text |
| ```geometry.create_signal_2d(n=100,...)``` 		| Text |
| ```geometry.demo_1(n=100)``` 		| Text |
| ```geometry.demo_2()``` 		| Text |
| ```geometry.demo_3(seed=1)``` 		| Text |
| ```geometry.dir_vectors(V,...)``` 		| Text |
| ```geometry.divide_space(X,...)``` 		| Text |
| ```geometry.downsampling_space(X,...)``` 		| Text |
| ```geometry.downsampling_surface_points(V,...)``` 		| Text |
| ```geometry.ds_mapping(X,...)``` 		| Text |
| ```geometry.ellipj_clx(u,...)``` 		| Text |
| ```geometry.filterDC_sGolay(X,...)``` 		| Text |
| ```geometry.find_E1inE2(E1_xy,...)``` 		| Text |
| ```geometry.forceUnitCircle(X)``` 		| Text |
| ```geometry.getEdges_idx(tri)``` 		| Text |
| ```geometry.getEdges_idxSet(tri)``` 		| Text |
| ```geometry.getTriFaces(V,...)``` 		| Text |
| ```geometry.getTriFaces_V2(V,...)``` 		| Text |
| ```geometry.get_PCA(X,...)``` 		| Text |
| ```geometry.get_adjacency_matrix_depth(V,...)``` 		| Text |
| ```geometry.get_adjacency_matrix_dist(V,...)``` 		| Text |
| ```geometry.get_boundary_points(XY)``` 		| Text |
| ```geometry.get_boundary_points_r(XY,...)``` 		| Text |
| ```geometry.get_boundary_v1(X,...)``` 		| Text |
| ```geometry.get_boundary_v2(X,...)``` 		| Text |
| ```geometry.get_center(X)``` 		| Text |
| ```geometry.get_circle(r=1,...)``` 		| Text |
| ```geometry.get_circular_grid(n=10,...)``` 		| Text |
| ```geometry.get_ellipsoid(n1=100,...)``` 		| Text |
| ```geometry.get_neibours(V,...)``` 		| Text |
| ```geometry.get_optimal_projection(X,...)``` 		| Text |
| ```geometry.get_plane(X,...)``` 		| Text |
| ```geometry.get_sphare(n1=100,...)``` 		| Text |
| ```geometry.get_square(n=5,...)``` 		| Text |
| ```geometry.get_square_grid(n=10,...)``` 		| Text |
| ```geometry.im2vec(file_name,...)``` 		| Text |
| ```geometry.indx2points_edges(xy,...)``` 		| Text |
| ```geometry.isEdge_inTri(T,...)``` 		| Text |
| ```geometry.lin_inter(x1,...)``` 		| Text |
| ```geometry.map_to_circle_v1(X,...)``` 		| Text |
| ```geometry.map_to_circle_v2(X,...)``` 		| Text |
| ```geometry.multi_plots(X,...)``` 		| Text |
| ```geometry.node2C_to_adjacency_matrix(node2C,...)``` 		| Text |
| ```geometry.opt_project(X,...)``` 		| Text |
| ```geometry.plot_map_2d(X,...)``` 		| Text |
| ```geometry.plot_proj(Xp,...)``` 		| Text |
| ```geometry.points_insideCurve(curvXY,...)``` 		| Text |
| ```geometry.project_on_hemisphere(X,...)``` 		| Text |
| ```geometry.removeTri_Edges(F,...)``` 		| Text |
| ```geometry.removeTri_edge(F,...)``` 		| Text |
| ```geometry.remove_long_edges_k(V,...)``` 		| Text |
| ```geometry.resize(image,...)``` 		| Text |
| ```geometry.rotation_matrix(theta=0.7853981633974483)``` 		| Text |
| ```geometry.selEdges(xy,...)``` 		| Text |
| ```geometry.spar2car(S)``` 		| Text |
| ```geometry.surface_plot_mayavi(V,...)``` 		| Text |
| ```geometry.surface_reconstruction(V,...)``` 		| Text |
| ```geometry.transform_image(X,...)``` 		| Text |
| ```geometry.transform_image_all(file,...)``` 		| Text |
| ```geometry.unwrape_3d(V,...)``` 		| Text |
| ```geometry.unwrape_surface(V,...)``` 		| Text |
| ```geometry.unwrape_surface_mirror(V,...)``` 		| Text |
| ```geometry.vec2im(X,...)``` 		| Text |


<h2 class="no-bg">Utils Module</h2>


| Syntax | Description |
| --- | ----------- |
| ```utils.ProgBar(i,...)``` 		| Text |
| ```utils.ProgBar_JL(i,...)``` 		| Text |
| ```utils.ProgBar_float(i,...)``` 		| Text |
| ```utils.ProgStatus(i,...)``` 		| Text |
| ```utils.entropy(x,...)``` 		| Text |
| ```utils.pretty_print(List,...)``` 		| Text |
| ```utils.print_list(L,...)``` 		| Text |
| ```utils.resize(image,...)``` 		| Text |
| ```utils.view_hierarchical_order(file_obj,...)``` 		| Text |
| ```utils.warning_on_one_line(message,...)``` 		| Text |



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
