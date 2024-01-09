# tinytapeout-kicad-libs

Symbols and footprints created to support TinyTapeout boards and extensions

The purpose of this repository is to serve as a single common location for kicad components that are use in multiple places throughout the TinyTapeout PCB ecosystem (e.g. the demo boards).


## Including the library in your project

If you are creating a project and would like to include the symbols and footprints, from within an 


  1) from within an initialized git repo run: `git submodule add https://github.com/tinytapeout/tinytapeout-kicad-libs.git`
  
  2) in kicad, use "Manage Symbol Libraries..." and "Manage Footprint Libraries..." to add project specific libraries
  
Ideally, that second step should use a relative/variable substitution path so that it will be portable to other systems, for example:
 
`${KIPRJMOD}/tinytapeout-kicad-libs/symbols/TinyTapeout.kicad_sym`


## Projects already using the library

For projects that use the library, clone the repo using the --recurse-submodules flag, e.g.

`git clone  --recurse-submodules https://github.com/psychogenic/whatever.git`

If you've already cloned a repository without using the flag, wind up with an empty stub (a directory without any contents) and would like to pull the contents to your local system, run

`git submodule update --init --recursive`

from within the project's top level directory.

