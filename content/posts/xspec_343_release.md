---
date: 2026-03-23
linktitle: Release XSpec v3.4.3
title: Release XSpec v3.4.3
weight: 6
categories: ["Release"]
tags: ["v3.4.3"]
---

<a href="https://github.com/xspec/xspec/issues/1766"><img align="right" src="https://user-images.githubusercontent.com/10128303/262700963-1a1e0fda-f335-4c90-9f8a-f72c5ece6c27.png" width="100px" alt="XSpec logo proposed and discussed in #1766"/>
</a>

## Release XSpec v3.4.3

XSpec 3.4 adds more entry points to the support for XQS as the Schematron implementation. These are the highlights of XSpec v3.4:

## Common to Languages Under Test

- After `x:context` or `x:call`, the `x:variable` and `x:like` elements can appear in any order and can be mixed. For example, the following sequence is valid: `x:call`, `x:variable`, `x:like`, `x:variable`, `x:like`
- Requires Java 17 or later. XSpec is tested with Java 17 and 21.
- Saxon 10 is no longer supported.
- XSpec is tested with XML Calabash v3.0.42.

## XSLT

- The "XSpec for XSLT using XProc" transformation scenario for Oxygen uses XProc v3.

## XQuery

- The "XSpec for XQuery using XProc" transformation scenario for Oxygen uses XProc v3.
- XSpec is tested with BaseX 12.2.

## Schematron

- If your Schematron schema uses an XQuery-based `queryBinding` (e.g., `queryBinding="xquery31"`), there are now more ways to execute an XSpec test for that schema. In v3.3, you can run such a test only with XProc. In v3.4, you can also run the test with `xspec.bat`, `xspec.sh`, Ant, or the "Run XSpec Test" transformation scenario. A local installation of [BaseX](https://basex.org/) is required. To learn more, see [Getting Started with XSpec and Schematron](https://github.com/xspec/xspec/wiki/Getting-Started-with-XSpec-and-Schematron) and [Schematron implementation](https://github.com/xspec/xspec/wiki/Requirements#schematron-implementation).
- The built-in XQS library is v1.1.5.

Many thanks to all the XSpec contributors who made this release possible! They are listed in the [release notes](https://github.com/xspec/xspec/releases/tag/v3.4.3).
