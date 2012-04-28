====================================
PyNE: Python for Nuclear Engineering
====================================

:Author: Anthony Scopatz <scopatz@gmail.com>
:Affiliation: The University of Chicago

PyNE, or `Python for Nuclear Engineering`_, is a nascent free and open source 
C++/Cython/Python package for performing common nuclear engineering tasks.  
This is intended as a base-level tool kit - akin to SciPy or Biopython - for 
common algorithms inside of the nuclear science and engineering domain.  

While PyNE may be considered long overdue from an external perspective, the 
nuclear industry poses a uniquely high barrier to entry for free software.  
That closed source solutions are often easier to develop is an irony that 
increases the noevlety of this package.

An intial hurdle for PyNE is the myriad of arcane file formats (both plaintext
and binary) which have been industry standard since the 1960s.  Though obtuse 
specifications are not soley a nuclear problem, the scale of the number of formats 
is much greater.  Partly to blame is that some of these formats were enshrined 
in international law at a time when Fortran 2 was the language of choice.

However, the main challenge for the community of PyNE developers is maintaining
the BSD license while explicitly avoiding any code which may be subject to 
export control.  Many nuclear engineering codes are open source in the sense
that the source code is distributed to developers who are then free to modify it.
However, due to the fear of illict use for the development of weapons, these
same codes are heavily export controlled and redistribution in any form is 
against their license.

This talk will contain an overview of the current capabilites of PyNE, 
a discussion of the export control issues mentioned above, a related 
discussion on the redistribution of raw nuclear data, and how the PyNE
team has been sucessful in developing highly performant tools to their
peers.

.. _Python for Nuclear Engineering: http://pyne.github.com/

...............................................................

Please indicate with an X your preference::

  [ ] Only consider this presentation for a talk.

  [ ] Only consider this presentation for a poster.

  [X] Consider this presentation for either a talk or a poster.

...............................................................

Please indicate with an X whether you are willing to prepare an
accompanying paper::

  [X] Yes  [ ] No

...............................................................

Optional: Indicate your preference for a specialized main track::

  [ ] High Performance Computing with Python
  [ ] Visualization

Or for one of the smaller domain-specific sessions::

  [ ] Computational bioinformatics
  [ ] Meteorology and climatology
  [ ] Astronomy and astrophysics
  [ ] Geophysics

Please note that this selection is simply a guideline for the program
committee, and that talks may be scheduled in a different session than
indicated.

...............................................................

Please email this form to 2012submissions@scipy.org
