---
date: 2023-10-01
linktitle: Release XSpec v2.3.2
title: Release XSpec v2.3.2
weight: 6
categories: [ "Release" ]
tags: ["v2.3.2"]
---

<a href="https://github.com/xspec/xspec/issues/1766"><img align="right" src="https://user-images.githubusercontent.com/10128303/262700963-1a1e0fda-f335-4c90-9f8a-f72c5ece6c27.png" width="100px" alt="XSpec logo proposed and discussed in #1766" /></a>

## Release XSpec v2.3.2
Release v2.3 fixes bugs, updates dependencies, and includes some refactoring. These are the highlights for XSpec v2.3.2:

#### Common to Languages Under Test

- Saxon 9.8 is no longer supported.
- XSpec is now tested with Saxon 12, 11, 10, and 9.9, while Saxon 9.9 is deprecated.
- Command line support fixes a bug that produced the wrong `XSPEC_HOME` value.

#### Schematron

- Ant performs some preprocessing in parallel, improving performance.

Many thanks to the many XSpec contributors who made this release possible. They are listed in the [release notes](https://github.com/xspec/xspec/releases/tag/v2.3.2).
