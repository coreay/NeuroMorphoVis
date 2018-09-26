# Input / Output Panel

![](images/io-1.png "NeuroMorphoVis")

## Summary
Use the input / output panel to set the input files and the output directories where the results will be generated.    

## Input Data Options 
The current version of NeuroMorphoVis can read morphologies stored in the following file formats:
+ The standard [.SWC](http://www.neuronland.org/NLMorphologyConverter/MorphologyFormats/SWC/Spec.html) file format. 
+ [H5](https://developer.humanbrainproject.eu/docs/projects/morphology-documentation/0.0.2/index.html) file format. This format is specific to the Blue Brain Project / Human Brain Projects, but the python bindings of HDF5 library must be installed to the system to load it.   

The users can select to load the morphologies from 
+ Individual .SWC or .H5 files based on their absolute pathes in the file system. In this case, the __Input Source__ option should be set to __H5 or SWC File__, and the path to the morphology file should be set in the __Morphology File__ text box. You can also use this button ![](images/io-button.png "") to open a file dialog to select the file from a specific path. 
+ A morphology linked to a certain neuron listed in a BBP circuit defined by its GID. 


The framework is mainly based on Blender. The current release uses the API of Blender 2.78b or 2.78c. Blender is a free software and can be downloaded from this [page](http://download.blender.org/release/). Blender comes with an LGPL license. 
There are other optional dependecies that are specific to users from [Blue Brain Project](https://github.com/BlueBrain). These dependencies are:
+ [HDF5 Python Bindings](https://www.h5py.org)
+ [Blue Brain Brion](https://github.com/BlueBrain/Brion) 


## Interfaces
NeuroMorphoVis is primarily designed as a plug-in in Blender. It comes with a user-friendly GUI and also with a rich set of command line options. Moreover, the tool is configurable via input configuration files making it possible to link it to web interface or using it on massively parallel visualization clusters for batch production.   

### GUI
![](images/neuromorphovis-interface.png "NeuroMorphoVis Interface")

### Command Line Options

### Modules 
NeuroMorphoVis comes with four principal modules for 
+ Data handling,
+ Simulation of three-dimensional somata profiles,
+ Building, repair and analysis of morphological skeletons,
+ Creation of piecewise-watertight polygonal surface meshes.

![## NeuroMorphoVis Interface](https://raw.githubusercontent.com/marwan-abdellah/NeuroMorphoVis/master/images/neuromorphovis-interface.png?token=ABOF06dhIj1X0w9k1PaZS85B3uMm6Mrpks5bqljtwA%3D%3D)

Neuronal soma reconstruction 
[![## Neuronal soma reconstruction](https://raw.githubusercontent.com/marwan-abdellah/NeuroMorphoVis/master/images/soma-reconstruction.png?token=ABOF04k9F31wN5-jtWAHsiE9SPMlFOHKks5bqliCwA%3D%3D)](https://www.youtube.com/watch?v=v02HogkFODU)

Morphology visualization 
[![## Neuronal morphology visualization](https://raw.githubusercontent.com/marwan-abdellah/NeuroMorphoVis/master/images/morphology-reconstruction.png?token=ABOF02GEsx4wN532esd5LAyhcAvYtDbBks5bqli3wA%3D%3D)](https://www.youtube.com/watch?v=74PGirMx3ks&t=102s)

Neuronal mesh reconstruction 
[![## Neuronal mesh reconstruction](https://raw.githubusercontent.com/marwan-abdellah/NeuroMorphoVis/master/images/mesh-generation.png?token=ABOF01D3_z8hCR2A4nZaPPm0gdj9R1yDks5bqljHwA%3D%3D)](https://www.youtube.com/watch?v=oxCKwrZSV98&t=130s)

![](images/mesh-generation.png "Vanilla GAN")




![](images/output.gif "Vanilla GAN")

### Morphology Shading Styles
The users can select to visualize and render the morphologies in different styles based on a set of shaders that are customized and adapted to create high quality images for illustrative purposes or scientitifc publications. 

![](images/morphology-shading-styles.png "Morphology Shading Styles")


## Publication & Citation 
If you use NeuroMorphoVis for your research, media design or other purposes, please cite our paper [NeuroMorphoVis: a collaborative framework for analysis and visualization of neuronal morphology skeletons reconstructed from microscopy stacks](https://academic.oup.com/bioinformatics/article/34/13/i574/5045775) using the following entry:

```
@article{abdellah2018neuromorphovis,
  title={NeuroMorphoVis: a collaborative framework for analysis and visualization of neuronal morphology skeletons reconstructed from microscopy stacks},
  author={Abdellah, Marwan and Hernando, Juan and Eilemann, Stefan and Lapere, Samuel and Antille, Nicolas and Markram, Henry and Sch{\"u}rmann, Felix},
  journal={Bioinformatics},
  volume={34},
  number={13},
  pages={i574--i582},
  year={2018},
  publisher={Oxford University Press}
}
```