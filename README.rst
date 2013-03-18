==================================================
vlfeat-ctypes: minimal VLFeat interface for python
==================================================

This is a minimal port of a few components of the matlab interface of `the
vlfeat library <http://www.vlfeat.org>` for computer vision to Python.

vlfeat's core library is written in C. In practice, though, a significant
amount of the library lies in the MATLAB interface.
This project is a port of a few functions from that interface to python/numpy,
using ctypes. It contains only a few functions
(the ones needed for `py-sdm <http://github.com/dougalsutherland/py-sdm>`).
The process isn't very hard, it just takes some effort.
Patches adding additional functionality are welcome.

There's also a fork of vlfeat floating around that includes Boost::Python
wrappers. I couldn't get it to work, and didn't try too hard because I saw that
some of the functions I needed had significant amounts of matlab code anyway.
You might be more interested in it, though;
`Andreas Mueller's version <https://github.com/amueller/vlfeat/>`
appears to be the most recently updated.