# Find executable

D library for finding executable files using PATH environment variable.

[![Build Status](https://travis-ci.org/MyLittleRobo/findexecutable.svg?branch=master)](https://travis-ci.org/MyLittleRobo/findexecutable)

Originally this was a part of [standardpaths](https://github.com/MyLittleRobo/standardpaths) library. But I found need in this kind of functionality in my other projects that don't depend on standardpaths.

[Online documentation](https://mylittlerobo.github.io/findexecutable/findexecutable.html)

## Examples

### [Find executable](examples/findexecutable/source/app.d)

Takes the name of executable as command line argument and searches PATH environment variable for retrieving absolute path to file. On Windows it also tries all known executable extensions.

    dub run :findexecutable --build=release -- whoami dub dmd
    