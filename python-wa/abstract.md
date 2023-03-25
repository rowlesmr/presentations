# I made a thing: Visualising powder X-ray diffraction data and models

### Matthew Rowles
### Adjunct Research Fellow, Curtin University


TL;DR: A short background on powder diffraction and data formats will be given. `pdCIFplotter`, my program for visualising powder diffraction data, will be explained, discussed, and demonstrated. `pdCIFplotter` was originally written in Python 3.7, and is about to undergo a large refactoring of the internal data structures to more easily provide more front-end functionality.

---

X-ray powder diffraction (XRD) is an analytical technique used to identify, quantify, and solve the crystal structures of materials. It is a staple technique in university and industrial laboratories, and the wide availability of instrumentation and analysis software is matched only by the different formats in which the data and models are saved in. The problem of mutually unintelligible data formats is not limited to diffraction data, but the crystallographic community has produced a solution.

The Crystallographic Information Framework (CIF) is a human- and machine-readable text-based file format for the exchange of crystallographic information. Originally constructed for single-crystal data, the core CIF dictionary has been extended to include powder diffraction data – pdCIF – amongst others. 

There are a variety of tools available for the creation, viewing, and editing of CIF files; however, there is a dearth of end-user tools that work well with pdCIF, and, as a result, the adoption of pdCIF is not as widespread as it should be. Common powder diffraction analysis software packages are often capable of outputting diffraction data and model results in pdCIF format but are then not able to read in those same files. This lack of interoperability makes studying the data and models by a third party a difficult process without access to the original software and analysis files. 

To expand the available pdCIF software tools for the end-user, the program `pdCIFplotter` has been written to provide an easy-to-use interface for visualizing powder diffraction data and models published in pdCIF format. In particular, support for the visualization of multi-pattern data sets, such as *in situ* data, is provided by means of stack and surface plots.

If you’re really keen, you can read ahead at https://doi.org/10.1107/S1600576722003478 and https://github.com/rowlesmr/pdCIFplotter. 

---

Matthew Rowles studied physics and materials science at Curtin University. After completing his PhD in 2005, he held two Postdoctoral Fellowships at the CSIRO where he learnt The Good Thing™ that is X-ray diffraction quantitative phase analysis, after which he sold electron-microscopy-adjacent paraphernalia for a short while. When that company got sold out from under his feet, he looked after X-ray diffraction laboratories at a couple of universities, and taught materials science, physics, and diffraction for a few years. He is currently a Technical Specialist (Diffraction and Spectroscopy) with Intertek Minerals, working on the quantitative analysis of X-ray diffraction and infra-red data. He is also (con)currently an Adjunct Research Fellow at Curtin University, maintaining contact with the central analytical facilities. He writes code like a scientist.
