---
date: 2026-06-01
linktitle: Release XSpec v4.0.2
title: Release XSpec v4.0.2
weight: 6
categories: ["Release"]
tags: ["v4.0.2"]
---

<a href="https://github.com/xspec/xspec/issues/1766"><img align="right" src="https://user-images.githubusercontent.com/10128303/262700963-1a1e0fda-f335-4c90-9f8a-f72c5ece6c27.png" width="100px" alt="XSpec logo proposed and discussed in #1766"/>
</a>

## Release XSpec v4.0.2

XSpec 4.0 supports testing your [XProc 3](https://xproc.org) code and enhances the XProc harness for running test suites. These are the highlights of XSpec v4.0:

## Common to Languages Under Test
* The XProc 3 pipelines for running XSpec tests can produce JUnit reports on the new
        `junit` output port. To produce JUnit reports, set the `junit-enabled` option to `'true'`.
* The XProc 3 pipelines for running XSpec tests have a new `inline-css` option with default
        value `'true'`, making the HTML report of test results a self-contained file. 
        **Compatibility Note:** The HTML report file is larger due to embedded CSS. For the
        XSpec v3 behavior, set `inline-css` to `'false'`.
* XSpec is tested with XML Calabash 3.0.47.

## XQuery
* XSpec is tested with BaseX 12.4.

## Schematron
* SchXslt2 v1.10.3 replaces SchXslt, for testing Schematron schemas having an XSLT-based queryBinding.

### Compatibility Notes

1. To specify a Schematron phase in your test, use a global `x:param` element. With SchXslt2,
        the parameter name is `Q{http://dmaus.name/ns/2023/schxslt}phase`, not `phase`.

2. SchXslt usage in XSpec is [deprecated but still works](https://github.com/xspec/xspec/wiki/Using-Another-Implementation-of-Schematron#using-schxslt-with-xspec-v232-and-earlier-or-v40-onward).

## XProc
* You can test your custom XProc 3 steps using XSpec and XML Calabash 3. You can execute your test suite from XML Calabash 3, Ant, or a shell/batch script. To learn more, see [Getting Started with XSpec for Testing XProc](https://github.com/xspec/xspec/wiki/Getting-Started-with-XSpec-for-Testing-XProc).

Many thanks to all the XSpec contributors who made this release possible! They are listed in the [release notes](https://github.com/xspec/xspec/releases/tag/v4.0.2), plus additional contributions to the XSpec 4.0 software and wiki documentation were made by @birdya22, @cmarchand, and @AirQuick.
