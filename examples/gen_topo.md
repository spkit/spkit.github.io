---
title: Generating Topographical Map
layout: default
---

# {{ page.title }}


## Generating Spatio-Temporal Map

Map at every time point x(t)

### At t=0, X[0]

```python
import spkit as sp
import matplotlib.pyplot as plt

X,ch_names = sp.load_data.eegSample()


Zi = sp.eeg.TopoMap(pos,X[0],res=128, showplot=True,axes=None,contours=True,showsensors=True,
            interpolation=None,shownames=True, ch_names=ch_names,showhead=True,vmin=None,vmax=None,
            returnIm = False,fontdict=None)
plt.show()    
```    

<img src = "figures/eeg_topo_1.png" >

```python
plt.imshow(Zi,cmap='jet',origin='lower')

```
<img src = "figures/eeg_topo_sqr_1.png" >


Map at every time point x(t)

### At t=0, X[0] with colorbar

```python
import numpy as np
import matplotlib.pyplot as plt
import spkit as sp

X,ch_names = sp.load_data.eegSample()


Zi,im = sp.eeg.TopoMap(pos,X[0],res=128, showplot=True,axes=None,contours=True,showsensors=True,
            interpolation=None,shownames=True, ch_names=ch_names,showhead=True,vmin=None,vmax=None,
            returnIm = True,fontdict=None)

plt.colorbar(im)
plt.show()    
```    

<img src = "figures/eeg_topo_2.png" >

```python
im = plt.imshow(Zi,cmap='jet',origin='lower')
plt.colorbar(im)
plt.show() 

```

<img src = "figures/eeg_topo_sqr_2.png" >



## Generating Spatio-Spectral Map

### For Three different frequency Bands

```python
fBands =[[4],[4,8],[8,14]]
Px = sp.eeg.RhythmicDecomposition(X,fs=128.0,order=5,Sum=True,Mean=False,SD=False,fBands=fBands)[0]
Px = 10*np.log10(Px)

fig = plt.figure(figsize=(15,4))
ax1 = fig.add_subplot(131)
Zi  = sp.eeg.TopoMap(pos,Px[0],res=128, showplot=True,axes=ax1,ch_names=ch,vmin=None,vmax=None)
ax1.set_title('<4 Hz')

ax2 = fig.add_subplot(132)
Zi  = sp.eeg.TopoMap(pos,Px[1],res=128, showplot=True,axes=ax2,ch_names=ch,vmin=None,vmax=None)
ax2.set_title('(4-8) Hz')

ax3 = fig.add_subplot(133)
Zi  = sp.eeg.TopoMap(pos,Px[2],res=128, showplot=True,axes=ax3,ch_names=ch,vmin=None,vmax=None)
ax3.set_title('(8-14) Hz')
plt.show()
```

<img src = "figures/eeg_ssfi_1.png" >       
