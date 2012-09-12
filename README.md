hls-fetch
=========

Introduction
------------

hls-fetch is a small program that downloads and decrypts HTTP Live Streaming (HLS) videos,
commonly used for streaming to Apple iOS devices.

It is written in Perl.

Author and Feedback
-------------------

hls-fetch is written by Oskar Liljeblad <oskar@osk.mine.nu>.

This software is a work in progress and there are probably many ways it can
still be improved. If you'd like to contribute patches, ideas, or bug
reports, please don't hesitate contacting me!

License
-------

hls-fetch is copyright (C) 2012 Oskar Liljeblad.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

Download
--------

The latest hls-fetch can be downloaded from GitHub:

 * <https://github.com/osklil/hls-fetch>

Requirements
------------

 * Perl 5.10.0 (or later)
   Debian: perl

 * OpenSSL (only needed for encrypted streams)
   Debian: openssl

 * HTML::Parser Perl module
   Debian: libhtml-parser-perl

 * LWP::UserAgent Perl module
   Debian: libwww-perl

 * JSON Perl module
   Debian: libjson-perl

 * URI Perl module
   Debian: liburi-perl

Usage
-----

All you need to specify on the command line is the URL to fetch.
hls-fetch will download the page and look for a <video> tag.
If you know the M3U playlist URL, then use the --playlist parameter
along with the URL to tell hls-fetch to download the playlist
directly.

Run 'hls-fetch --help' for further usage information.

Future
------

Nothing is planned for the future right now.

References
----------

 * HTTP Streaming with Encryption under Linux
   <http://www.opensolutions.ie/blog/2010/08/http-streaming-with-encryption-under-linux/>
