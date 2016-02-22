
.. _subpackages-label:

xSDK Packages
--------------------------

This lists the xSDK packages with a short discription of each

* Alquimia is an API for providing mature geochemistry and biogeochemistry 
  capabilities to reactive transport codes. It is not a geochemistry solver--it is 
  a library comprising data structures and interfaces that wrap chemistry solvers 
  from well-established codes like PFlotran (http://www.pflotran.org) and 
  CrunchFlow (http://www.csteefel.com/CrunchFlowIntroduction.html), 
  allowing developers of newer codes to use these solvers with a single interface. 
  We refer to these chemistry solvers as chemistry engines.

  Currently, Alquimia supports two chemistry engines: PFlotran and CrunchFlow. 
  There are plans to support more in the future, depending on funding and levels 
  of engagement in the DOE's reactive transport research community.

  You can find out more about programming with Alquimia at 
  https://www.github.com/LBL-EESA/alquimia-dev.

*  The  hypre software library provides high performance preconditioners and solvers for the solution of large sparse
   linear systems on massively parallel computers. It was created with the primary goal of providing users with advanced parallel preconditioners.
   The library features parallel multigrid solvers for both structured and unstructured grid problems. 
   For ease of use, these solvers are accessed from the application code via hypre's conceptual linear system interfaces,
   which allow a variety of natural problem descriptions and include a structured, a semi-structured interface, and a traditional
   linear-algebra based interface. The (semi-)structured interfaces are an alternative to the standard matrix-based interface that
   describes rows, columns, and coefficients of a matrix. Here, instead, matrices are described primarily in terms of stencils and
   logically structured grids. These interfaces give application users a more natural means for describing their linear systems,
   and provide access to methods such as structured multigrid solvers, which can take advantage of the additional information beyond just the matrix. 

  The library is written in C and has a Fortran interface. It supports MPI+OpenMP.
  More detailed information can be found at \cite{hypre_webpage, hypre_usr_manual}.
