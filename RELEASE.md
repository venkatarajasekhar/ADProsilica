ADProsilica Releases
==================

The latest untagged master branch can be obtained at
https://github.com/areaDetector/ADProsilica.

Tagged source code and pre-built binary releases prior to R2-0 are included
in the areaDetector releases available via links at
http://cars.uchicago.edu/software/epics/areaDetector.html.

Tagged source code releases from R2-0 onward can be obtained at 
https://github.com/areaDetector/ADProsilica/releases.

Tagged prebuilt binaries from R2-0 onward can be obtained at
http://cars.uchicago.edu/software/pub/ADProsilica.

The versions of EPICS base, asyn, and other synApps modules used for each release can be obtained from 
the EXAMPLE_RELEASE_PATHS.local, EXAMPLE_RELEASE_LIBS.local, and EXAMPLE_RELEASE_PRODS.local
files respectively, in the configure/ directory of the appropriate release of the 
[top-level areaDetector](https://github.com/areaDetector/areaDetector) repository.


Release Notes
=============

R2-0
----
* Moved the repository to [Github](https://github.com/areaDetector/ADProsilica).
* Re-organized the directory structure to separate the driver library from the example IOC application.
* Fixes for connection management to handle multiple cameras per IOC. Thanks to Kate Feng.
* Added ability to convert Bayer images to RGB1, RGB2, and RGB3 images.  This reduces the network
  bandwidth load at the expense of more CPU load on the IOC host machine.  In areaDetector releases
  prior to R-2.0 this capability existed in the NDPluginColorConvert plugin.  It has been removed
  from NDPluginColorConvert so that it would no longer depend on the AVT PvAPI library.


R1-9-1 and earlier
------------------
Release notes are part of the
[areaDetector Release Notes](http://cars.uchicago.edu/software/epics/areaDetectorReleaseNotes.html).