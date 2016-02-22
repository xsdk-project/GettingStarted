
.. _subpackages-label:

xSDK Packages
==================

This lists the xSDK packages with a short discription of each

Alquimia_
-----------------

.. _Alquimia: https://www.github.com/LBL-EESA/alquimia-dev

Provides an API for providing mature geochemistry and biogeochemistry 
capabilities to reactive transport codes. It is not a geochemistry solver--it is 
a library comprising data structures and interfaces that wrap chemistry solvers (called chemistry engines) 
from well-established codes like PFlotran (http://www.pflotran.org) and 
CrunchFlow (http://www.csteefel.com/CrunchFlowIntroduction.html), 
allowing developers of new codes to use these solvers with a single interface. 
We refer to these chemistry solvers as chemistry engines.


hypre_
---------------

.. _hypre: https://computation.llnl.gov/project/linear_solvers/software.php

Provides high performance preconditioners and solvers for the solution of large sparse
linear systems on massively parallel computers. It was created with the primary goal of providing users with advanced parallel preconditioners.
The library features parallel multigrid solvers for both structured and unstructured grid problems. 
For ease of use, these solvers are accessed from the application code via hypre's conceptual linear system interfaces,
which allow a variety of natural problem descriptions and include a structured, a semi-structured interface, and a traditional
linear-algebra based interface. The (semi-)structured interfaces are an alternative to the standard matrix-based interface that
describes rows, columns, and coefficients of a matrix. Here, instead, matrices are described primarily in terms of stencils and
logically structured grids. These interfaces give application users a more natural means for describing their linear systems,
and provide access to methods such as structured multigrid solvers, which can take advantage of the additional information beyond just the 
Supports C and Fortran. Can be used with OpenMP.

PETSc_
---------------

.. _PETSc: http://www.mcs.anl.gov/petsc

PETSc is a suite of data structures and routines for the scalable
solution of scientific applications modeled by partial differential
equations.  It includes linear solvers, preconditioners, nonlinear
solvers, and ODE integrators. It also provides a variety of scalable
constrained and unconstrained optimization solvers.  PETSc utilizes
the MPI program model and does not use threads.  While it does
not include eigensolvers, there is an eigensolver package called SLEPc
built on top of PETSc with a very similar interface. The library
libMesh and the framework MOOSE provide finite element solvers that
utilize PETSc.

SuperLU_Dist_
---------------

.. _SuperLU_Dist: http://crd-legacy.lbl.gov/~xiaoye/SuperLU/

SuperLU is a general purpose library for the direct solution of large,
sparse, nonsymmetric systems of linear equations on high performance
machines.  The library routines will perform an LU decomposition with
partial pivoting and triangular system solves through forward and back
substitution. The LU factorization routines can handle non-square
matrices but the triangular solves are performed only for square
matrices. The matrix columns may be preordered (before factorization)
either through library or user supplied routines. This preordering for
sparsity is completely separate from the factorization. Working
precision iterative refinement subroutines are provided for improved
backward stability. Routines are also provided to equilibrate the
system, estimate the condition number, calculate the relative backward
error, and estimate error bounds for the refined solutions.

There are three separate versions of this code: SuperLU (for sequential machines),
SuperLU_MT (for shared memory parallel machines with using OpenMP or Pthread), and
SuperLU_DIST (for distributed memory machines using MPI).

The library is written in C, with Fortran interface.  SuperLU_DIST supports MPI+X,
where X can be CUDA, OpenMP, or both.

Trilinos_
---------------

.. _Trilinos: http://trilinos.org

The Trilinos Project is an effort to develop algorithms and enabling
technologies within an object-oriented software framework for the solution of
large-scale, complex multi-physics engineering and scientific problems. Trilinos
is organized into 66 different packages, each with a specific focus.  These
packages include linear and nonlinear solvers, preconditioners (including
algebraic multigrid), graph partitioners, eigensolvers, and optimization
algorithms, among other things.  Users are only required to install the subset
of packages related to the problems they are trying to solve.

Trilinos supports MPI+X, where X can be CUDA, OpenMP, etc.
