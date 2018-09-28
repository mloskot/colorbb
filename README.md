colorbb
-------

This is a simple wrapper written in Perl for making the output from
`b2` command from [Boost.Build](http://http://www.boost.org/build/)
easier to read (more colorful), and errors easier to find
in messy compilations. Initially discussed as part of Boost trac ticket
[#3508 - bjam output in colours](https://svn.boost.org/trac10/ticket/3508).

Port of [colormake](http://bre.klaki.net/programs/colormake/)
by Bjarni R. Einarsson.

![screenshot](https://user-images.githubusercontent.com/80741/38137483-206a3034-3425-11e8-872c-4f95dd948df5.png "colorbb in action")



Files
-----

- `colorbb.pl`  A perl filter, which colorizes `b2` output.
- `colorbb`     A shell script, which combines `b2` and `colorbb.pl`

Install
-------

Copy both scripts to location in your `$PATH`.

Usage
-----

Type `colorbb` whenever you'd ordinarily type `b2`:

```console
$ colorbb -j4 toolset=clang cxxflags="-std=c++11" variant=debug test
```

Author
------

Mateusz Loskot, http://mateusz.loskot.net/.

Credits
-------

Bjarni R. Einarsson for
[colormake](http://bre.klaki.net/programs/colormake/).

License
-------

(inherited from colormake)

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.
