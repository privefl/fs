This should fix the malloc / delete inconsistency in the Valgrind and ASAN
issues in the CRAN checks. As directed by CRAN maintainers I am submitting ASAP
to avoid removal from CRAN on March 28th.

Apologies for the oversight and for the quick submissions.

## Test environments
* local OS X install, R 3.4.3
* ubuntu 14.04 (on travis-ci), R 3.4.3
* win-builder (devel and release)
* Solaris 10 (in a VM)

## R CMD check results

0 errors | 0 warnings | 1 note

* GNU make is a SystemRequirements.
  This is needed by the Makefile for the libuv dependency, it is not practical
  to convert this to a POSIX compatible Makefile.
