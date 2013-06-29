pat2pdf
=======

This script connects to the [USPTO](http://patft.uspto.gov/) patent database, retrieves the TIFF images of patents or patent applications and converts them into a single PDF file using libtiff.

Yes, I know, you would have written it in perl/python/(insert your favourite scripting language here), but it is written in shell and works well.

It requires an http fetcher (lynx by default), tiffcp and tiff2pdf (both part of libtiff).

History
======

This script was originally written by Oren Tirosh and Thomas Boege. In 2013 the script broke due to changes to the USTPO website. Paul William fixed the script and uploaded it to GitHub because its [original homepage](http://www.tothink.com/pat2pdf) was no longer online.

Usage
====

pat2pdf <number>|<application number>

Example
===

Fetching a USTPO patent application:

pat2pdf 20130049740

Fetching a USTPO patent:

pat2pdf 8259522

Result is a file in the current directory named pat<patnum>.pdf

License
======

This script is licensed under the GPL (version unspecified).
