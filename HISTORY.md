# HISTORY

This is a copy of the Open Motif repository at https://git.code.sf.net/p/motif/code .

That repo iswas maintained by ICS MotifZone: https://motif.ics.com/

This repo is an attempt to fix some things since it looks like ICS MotifZone isn't maintaining this any more.

The initial import from ICS is located in the motifzone branch. Any
further updates from them will be located there.  I would not hold my
breath.

Development in this repo will be done on the 'main' branch.

The idea here is to fix up things to make it easier to build on more
modern systems and allow greater participation of the development
community.


## 2.3.9 Release, 6/21/2026

The changes here are to fix up some build issues, get rid of
`register` declarations and a variety other minor issues.  This is the
first release based on the 2.3.8 Motif release that was being
maintained by ICS at:  https://sourceforge.net/projects/motif/

Note, there is a another Motif port being maintained at:
https://github.com/thentenaar/motif by Tim Hentenaar.

At some point, maybe the fixes in this repository should be passed
onto Tim.  No need for two Motif forks :)

For now, though I will release the current state of this Motif fork.

Short log:

```
Jon Trulson (18):
      Add a README.md
      README.md: update, add README, and remove README file
      Disable XPrinting by default
      Makefile.am files: replace ancient INCLUDES with current AM_CPPFLAGS
      Get autogen.sh to run without errors and warnings
      .gitignore: add more artifacts since we can now compile successfully
      Fix up library issues (libXt, primarily) so we can build successfully
      Remove all uses of the 'register' C keyword
      wml: use abs_srcdir instead of srcdir, rm srcdir where it isn't needed
      wml: fixup format-security and size_t format specifier warnings
      configure.ac: change the way LEX is detected
      wmluiltok.l: add a main() to avoid need for -ll or -lfl libs
      configure: freebsd: enable MTSAFE api, enable LIBICONV_PLUG
      autogen.sh: use m4 includes with aclocal rather than .
      iconv: add detection support for netbsd and others, remove obsolete configs
      libXm: add libiconv as needed as a dependent library
      Test a basic build workflow (#3)
      Fix a basic github workflow (#5)
```




