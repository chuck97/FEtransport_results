# Error values for Finite Element advection tests on sphere
This repository contains 2 files "TEST2" and " TEST3" that presents errors for advection tests (paper "The suite of Taylor-Galerkin class schemes for ice transport on sphere implemented by the INMOST package" by Sergey S. Petrov and Nikolay G. Iakovlev).

Test configuration:
1. Finite Element space discretization. Continuous Galerkin method with linear Lagrangian elements on triangle;
2. Time discretization - TG2 (Taylor-Galerkin method of 2 order), TTG2 (Two-step Taylor-Galerkin method of 2 order), TTG3 (Two-step Taylor-Galerkin method of 3 order), TTG4 (Two-step Taylor-Galerkin method of 4 order), with/without FCT (Flux correction method applied). See article for more details;
3. Mesh - regular sphere triangulation (with Earth radius) with ~200km triangle size;
4. Initial scalar distribution and velocity field (see article), TEST2 - SC+ND1, TEST3 - SC+ND2;
5. Total time integration - 300 hours;
6. Time step calculated through resolution, Courant number and max velocity.

Volocity fields are reversble so initial scalar distribution is equal to final one and exact solution is avalible.

In files l1 stands for l_1 error, l2 - l_2 error, linf - l_inf, max - phi_max error, min - phi_min error.
