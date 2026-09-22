---
title: SharpEyes
date: 2021-01-31
links:
  - type: code
    url: https://github.com/gallantlab/sharpeyes
  - type: site
    url: https://gallantlab.org/SharpEyes/

featured: true
---
Eye movements are the first action in the perception-cognition-action loop, and in an interactive experiment participants look wherever they choose. Any model of visual representaitons in the brain from such data must therefore be built in the coordinate frame of the retina rather than the screen. 

SharpEyes provides a suite of capabilities for eyetracking video analysis and for building motion-energy features from stimulus video. It detects pupils from video freames, maps pupil position to gaze position, recenters stimulus screen recordings to retinotopic coordinates, and provides an interface to [https://github.com/gallantlab/pymoten](pymoten) to compute motion-energy features from these stimulus videos. In addition to processing raw pupil video recordings, SharpEyes can also directly read `.edf` files produced by SR Research Eyelink systems (the user must supply the Eyelink SDK dll files).

At all steps, SharpEyes provides an interface for reviewing its outputs and correcting them by hand to ensure data quality. 

Precompiled builds are available for Windows and Linux.
