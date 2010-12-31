#TODO

##Dependencies
__boost__ depends on __bzip2__. I have added a <code>DEPEND=bzip2</code> variable in boost's build script, but currently it is not used. I should probably write a small dependency-checking script.

##Documentation
TODO: write this to-do. Just joking…

##Universal static libraries
Do we want them? Some library could have automatically generated public headers depending on the platform.

##Future
Libraries to be added in near future:

* ICU
* [FreeImage](http://freeimage.sourceforge.net/): depends on LibTIFF, LibJPEG, LibPNG, LibMNG, ZLib, OpenEXR, OpenJPEG and LibRaw-Lite.
* [Object-oriented Input System](http://sourceforge.net/projects/wgois/reviews/)
* [libtxc_dxtn](http://homepage.hispeed.ch/rscheidegger/dri_experimental/s3tc_index.html) (remove divisions and decode pixel blocks + use std types rather than GL types)
* [Tremor](http://wiki.xiph.org/Tremor), or rather my ARM-optimized version.
    * Maybe merge my changes with RockBox's version at <code>svn://svn.rockbox.org/rockbox/trunk</code> ?
* [TheorARM](http://wss.co.uk/pinknoise/theorarm/)
* [TinyVector](http://code.google.com/p/tinyvector/)
* [TinyXML](http://www.grinninglizard.com/tinyxml/)
* [OpenCollada](http://code.google.com/p/opencollada/)
* [VectorMathLib](http://code.google.com/p/bullet/)
* [Dynamica plugin](http://code.google.com/p/dynamica/)
* expat
* OpenCV
* [FLANN](http://www.cs.ubc.ca/~mariusm/index.php/FLANN/FLANN)
* [OpenKinect](http://openkinect.org/)
* O3D


