# This is a branch of GCC 11-3 with experimental support for AArch64 (Arm64) on Darwin.

The branch is recommended for (and has been tested on) powerpc, i686, x86_64 and aarch64 Darwin from Darwin9 (Mac OSX 10.5) through Darwin21 (macOS 12) (for architectures relevant to each version). The branch has also been tested to build cross-compilers between x86_64 and aarch64 and on aarch64-linux-gnu without regressions.

The branch contains a number of back-ports from GCC master that are required for Arm64 support and recommended for other Darwin architectures.  _Some of these are not suitable for application to the upstream branch and therefore will only be available on the Darwin-specific branch_.

The support for Aarch64 (Arm64) remains experimental but is adequate now for many programs (and self-bootstrap).

Please see README for general information on the GCC sources.

Please see the GCC 11.3 release documentation for the implementation status of core language features.

Please see gcc/config/aarch64/darwinpcs.md for a description of the macOS AArch64 (Arm64) ABI support.

Please report issues for this branch to: https://github.com/iains/gcc-11-branch/issues

**_The current release is GCC-11.4-darwin-r0. (May 2023)_**

This release:
 * Includes all upstream fixes.
 * All fixes in previous releases and on the GCC-12 branch.

Thanks to contributors and testers.

Release GCC-11.3-darwin-r1 (May 2022).

 * Fix missing __float128 support in libgfortran.

Release GCC-11.3-darwin-r0 (May 2022).

Test results : https://github.com/iains/gcc-11-branch/issues/1#issue-1228803806

Thanks to:

'FX' (https://github.com/fxcoudert) for the main part of the ```__float128``` support, many test fixes and help in testing this release more widely.
Andrew Burgess (while at Embecosm) for the work on heap based trampolines.
Maxim Blinov (Embecosm) for work on modifications to GCC's function lowering code to enable better support of the Darwin Arm64 ABI.

Iain Sandoe, May 2022
