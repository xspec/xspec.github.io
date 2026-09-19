---
date: 2026-09-22
linktitle: Release XSpec v4.1.2
title: Release XSpec v4.1.2
weight: 6
categories: ["Release"]
tags: ["v4.1.2"]
---

<img align="right" src="https://github.com/xspec/xspec/blob/main/graphics/xspec-logo.svg" width="100px" alt="XSpec logo"/>

## Release XSpec v4.1.2

XSpec 4.1 supports testing XProc using MorganaXProc-IIIee and running tests for Schematron using an XProc pipeline. These are the highlights of XSpec v4.1:

## Common to Languages Under Test
* XSpec is tested with Saxon 12.10 and 13.0.
* XSpec is tested with XML Calabash 3.0.54.
* Saxon 11 is no longer supported.
* XProc 1 is no longer supported.

## XSLT
* The code coverage feature has minor changes to make it compatible with Saxon 13.0 as well as Saxon 12.7 through 12.10 ([#2377](https://github.com/xspec/xspec/issues/2377)).

## Schematron
* You can use an XProc 3 pipeline to execute an XSpec test for a Schematron schema that has an XSLT-based queryBinding. Instructions are in the [XSpec wiki](https://github.com/xspec/xspec/wiki/Running-with-XProc#xspec-test-for-schematron-with-xproc-3-and-xslt-based-implementation-of-schematron). The case of XQuery-based queryBinding has been supported since v3.3.
* The built-in SchXslt2 library is v1.11.2.

## XProc
* You can execute a test for XProc with either MorganaXProc-III Extended Edition (new in v4.1) or XML Calabash 3 (since v4.0). Both processors support executing your test suite from XProc, Ant, or a shell/batch script. For details, see [XSpec test for XProc with XProc 3 and MorganaXProc-IIIee XProc processor](https://github.com/xspec/xspec/wiki/Running-with-XProc#xspec-test-for-xproc-with-xproc-3-and-morganaxproc-iiiee-xproc-processor) or other [mentions of MorganaXProc](https://github.com/search?q=repo%3Axspec%2Fxspec+MorganaXProc&type=wikis) in the XSpec wiki.
* Support for testing XProc is tested with MorganaXProc-IIIee 1.8.17 and XML Calabash 3.0.54.

Many thanks to all the XSpec contributors who made this release possible! They are listed in the [release notes](https://github.com/xspec/xspec/releases/tag/v4.1.2).
