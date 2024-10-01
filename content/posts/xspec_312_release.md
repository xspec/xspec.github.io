---
date: 2024-09-30
linktitle: Release XSpec v3.1.2
title: Release XSpec v3.1.2
weight: 6
categories: ["Release"]
tags: ["v3.1.2"]
---

<a href="https://github.com/xspec/xspec/issues/1766"><img align="right" src="https://user-images.githubusercontent.com/10128303/262700963-1a1e0fda-f335-4c90-9f8a-f72c5ece6c27.png" width="100px" alt="XSpec logo proposed and discussed in #1766" /></a>

## Release XSpec v3.1.2

XSpec 3.1.2 fixes bugs in the coverage status shown in XSLT code coverage reports. This release also updates dependencies. These are the highlights of XSpec v3.1:

#### Common to Languages Under Test

- XSpec is tested with Saxon 12.5, except that the detailed contents of XSLT code coverage reports are tested with Saxon 12.4.
- The XSpec schemas enforce the boolean values for the `x:expand-text` attribute and provide a Schematron Quick Fix for `expand-text` attributes on non-XSpec elements.

#### XSLT

- XSLT code coverage reports include a new coverage status of "unknown" for situations where XSpec has insufficient data to judge whether a node was hit or missed. Some instances of hit/miss/unknown determinations differ based on the Saxon version used for generating the report. While both Saxon 12.4 and 12.5 are supported, 12.4 is currently preferred for coverage reporting.

#### XQuery

- XSpec is tested with BaseX 11.3.

#### Schematron

- SchXslt 1.10 replaces SchXslt 1.9.5 as the built-in Schematron implementation.

Many thanks to all the XSpec contributors who made this release possible! They are listed in the [release notes](https://github.com/xspec/xspec/releases/tag/v3.1.2).
