---
title: Generating Topographical Map
layout: default1
---

# {{ page.title }}


## code

```python
import spkit as sp
import matplotlib.pyplot as plt

X,ch_names = sp.load_data.eegSample()


Zi = sp.eeg.TopoMap(pos,X[0],res=128, showplot=True,axes=None,contours=True,showsensors=True,
            interpolation=None,shownames=True, ch_names=ch,showhead=True,vmin=None,vmax=None,
            returnIm = False,fontdict=None)
plt.show()    
```    


<img src = "assets/images/eeg_topo_1.png" >

```python
plt.imshow(Zi,cmap='jet',origin='lower')

```
<img src = "assets/images/eeg_topo_sqr_1.png" >
