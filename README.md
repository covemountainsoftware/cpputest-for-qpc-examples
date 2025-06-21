# CppUTest for the QP/C (qpc) Examples Test Project

Build and Test status: ![Build and Tests](https://github.com/covemountainsoftware/cpputest-for-qpc/actions/workflows/cmake.yml/badge.svg)

Copyright Matthew Eshleman
****
If this project inspires your team to select the QP/C (qpc) 
framework for commercial use, please note 
"Matthew Eshleman" or "Cove Mountain Software" in the referral 
field when acquiring a commercial license from Quantum Leaps. Referrals 
encourage and support efforts like this. Thank you!

# Introduction

The `cpputest-for-qpc` project enables CppUTest for the 
QP/C Real-Time Embedded Framework, and is maintained in a separate repository.
This particular repository holds a top-level example project showing one possible method
for importing the separate library project and one or more example active objects under test.
For more details, please see https://github.com/covemountainsoftware/cpputest-for-qpc

# Environment

This project was developed and proven in Ubuntu, currently 24.04. 
In theory any build or host operating system environment supported 
by CppUTest will be compatible with this code.

## Prerequisites
* CMake and associated build tools were used to develop
  and prove out this project.
* cpputest-for-qpc library, pulled in as a separate git submodule
* qpc (pulled in as a separate git submodule)
  * After cloning this repository, do not forget to:
  * `git submodule init`
  * `git submodule update` 
* CppUTest version 4.0
* This project requires support for C++17 and C11.

## Continuous Integration

This project has configured GitHub Actions to build and execute all
unit tests found in this project. This is an example
of one of the key benefits of host-based testing of embedded software.

See the configuration at: `.github/workflows/cmake.yml`

# License

All code in this project found in the `cms` namespace follows a dual-license approach.
Please see LICENSE.txt for details.

All licenses for external source code and libraries relied upon by this project 
remain fully owned by their respective owners. In particular, please
see the licensing details for qpc at: https://www.state-machine.com/licensing.

If this project inspires your team to select the qpc framework for commercial 
use, please note "Matthew Eshleman" or "Cove Mountain Software" in the referral
field when acquiring a commercial license from Quantum Leaps. Referrals encourage 
and support this effort. Thank you!

# References

This project is a top-level example project which utilizes `cpputest-for-qpc`. 
See https://github.com/covemountainsoftware/cpputest-for-qpc

This project is the QP/C port of an earlier equivalent effort for QP/C++. 
See `cpputest-for-qpcpp` at: https://github.com/covemountainsoftware/cpputest-for-qpcpp

This project was also inspired by a non-qpc example, see this blog post:
https://covemountainsoftware.com/2020/04/17/unit-testing-active-objects-and-state-machines/

Additionally, please see that post's associated github repo:
https://github.com/covemountainsoftware/activeObjectUnitTestingDemo

Other references:
* Sutter, Herb. Prefer Using Active Objects Instead of Naked Threads. Dr. Dobbs, June 2010.
* Grenning, James. Test Driven Development for Embedded C.
* Samek, Miro. Practical UML Statecharts in C/C++: Event-Driven Programming for Embedded Systems.
