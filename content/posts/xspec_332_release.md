---
date: 2025-09-25
linktitle: Release XSpec v3.3.2
title: Release XSpec v3.3.2
weight: 6
categories: ["Release"]
tags: ["v3.3.2"]
---

<a href="https://github.com/xspec/xspec/issues/1766"><img align="right" src="https://user-images.githubusercontent.com/10128303/262700963-1a1e0fda-f335-4c90-9f8a-f72c5ece6c27.png" width="100px" alt="XSpec logo proposed and discussed in #1766"/>
</a>

## Release XSpec v3.3.2

XSpec 3.3 upgrades its XProc harnesses to XProc 3 and adds support for XQS as the Schematron implementation. These are the highlights of XSpec v3.3:

## Common to Languages Under Test

- In the `x:expect` element, the new, optional `result-type` attribute describes the sequence type you expect for the actual result. XSpec checks the type before evaluating `@test`, so an unexpected type leads to an ordinary failure instead of a type error.
- XSpec reports its own version number in command-line output and HTML reports.
- This will be the last XSpec release to support Java 8.
- This will be the last XSpec release to support Saxon 10 and Saxon 11.


## XSLT

- You can execute an XSpec test for XSLT using an XProc 3 pipeline.

## XQuery
- You can execute an XSpec test for XQuery using an XProc 3 pipeline.
- XSpec is tested with BaseX 12.0.

## Schematron
- You can execute an XSpec test for a Schematron schema that uses an XQuery-based `queryBinding`, using XQS as the Schematron implementation. _Initial limitation_: Access to this feature is via XProc 3 only.


Many thanks to all the XSpec contributors who made this release possible! They are listed in the [release notes](https://github.com/xspec/xspec/releases/tag/v3.3.2).
