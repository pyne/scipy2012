====================================
PyNE: Python for Nuclear Engineering
====================================

:Author: Anthony Scopatz <scopatz@gmail.com>
:Affiliation: The University of Chicago

:Author: Paul Romano <paul.k.romano@gmail.com>
:Affiliation: Massachusetts Institute of Technology

:Author: Paul Wilson <uwgonuke@gmail.com>
:AFfiliation: University of Wisconsin-Madison


PyNE, or `Python for Nuclear Engineering`_, is a nascent free and open source 
C++/Cython/Python package for performing common nuclear engineering tasks.  
This is intended as a base-level tool kit - akin to SciPy or Biopython - for 
common algorithms inside of the nuclear science and engineering domain.  

While PyNE may be considered long overdue from an external perspective, the 
nuclear industry poses a uniquely high barrier to entry for free software.  
That closed source solutions are often easier to develop is an irony that 
increases the novelty of this package.

An initial hurdle for PyNE is the myriad of arcane file formats (both plain text
and binary) which have been industry standard since the 1960s.  Though obtuse 
specifications are not solely a nuclear problem, the scale of the number of formats 
is much greater.  Partly to blame is that some of these formats were enshrined 
in international law at a time when Fortran 2 was the language of choice.

Thus the emerging value of PyNE is that it allows new users to shortcut the tedious and 
error prone process of writing their own tools to parse these obtuse data and output file 
formats.  The current unfortunate state of affairs is due in part to huge institutional 
inertia on the part of the maintainers of such formats.  This manifests as a reluctance to 
develop or refactor new and existing codes in a modern open source manner.  PyNE seeks to 
gain human efficiency via a shared set of solutions rather than having every developer 
around the world replicate the same parsing routines.

Another major challenge for the community of PyNE developers is maintaining
the BSD license while explicitly avoiding any code which may be subject to 
export control.  Many nuclear engineering codes are open source in the sense
that the source code is distributed to developers who are then free to modify it.
However, due to the fear of illicit use for the development of weapons, these
same codes are then heavily export controlled and redistribution in any form is 
against their licenses and is likely illegal.

Redistribution concerns are not limited to source code.  Basic nuclear data, 
while fundamentally un-copywritable under Western jurisprudence, also 
be considered sensitive and subject to export control laws.  PyNE has developed
a three-tiered strategy to alleviate the data burden of the individual user based 
on the level of openness of the data. 

In spite of the above administrative concerns, PyNE's place in the nuclear ecosystem
requires it have a general architecture.  Large portions of the code base are 
written in pure C or C++ and are built as Python-independent shared libraries. This
enables other, compiled nuclear engineering codes to leverage PyNE.  Hence, the 
Cython layer has wrappers for C++ standard library containers (maps, 
sets, lists, etc) which implement the ``collections`` interface of the 
appropriate type.  Because of the high degree of factorization in PyNE, these wrappers 
could easily be reused by other projects.

This talk will contain an overview of the current capabilities of PyNE, 
a discussion of the export control issues, a related 
discussion on the redistribution of raw nuclear data, and how the PyNE
team has been successful in developing highly performant tools for themselves and
their peers.

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
