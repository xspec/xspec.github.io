---
date: 2024-04-17
linktitle: Release XSpec v3.0.3
title: Release XSpec v3.0.3
weight: 6
categories: [ "Release" ]
tags: ["v3.0.3"]
---

<a href="https://github.com/xspec/xspec/issues/1766"><img align="right" src="https://user-images.githubusercontent.com/10128303/262700963-1a1e0fda-f335-4c90-9f8a-f72c5ece6c27.png" width="100px" alt="XSpec logo proposed and discussed in #1766" /></a>

## Release XSpec v3.0.3
Release v3.0.3 upgrades its connections with related software. Support for testing Schematron schemas now uses SchXslt as the built-in Schematron implementation. XSLT code coverage is compatible with Saxon 12.4 or later. These are the highlights of XSpec v3.0:

#### Common to Languages Under Test

- XSpec is tested with Saxon 12, 11, and 10, while use of Saxon versions earlier than 12.4 is not recommended.
- XSpec no longer supports Saxon 9.
- When comparing XML, you can ignore some or all attributes using three-dot syntax `x:attrs="..."`.
- XPath function items stored in global variables are testable using syntax `<x:call function="my-function" call-as="variable">`.

#### XSLT

- XSLT code coverage feature is compatible with Saxon 12.4. **Compatibility note:** This upgrade is not backward compatible with earlier Saxon versions. Also, Saxon 12.4 does not report some `xsl:sequence` instructions that are actually hit.
- XSpec experimentally supports testing with XSLT 4.0 and XPath 4.0. Set `xslt-version="4.0"` on `x:description`, and use an XSLT processor that has support for 4.0 enabled.

#### XQuery

- XSpec experimentally supports testing with XQuery 4.0 and XPath 4.0. Set `xquery-version="4.0"` on `x:description`, and use an XQuery processor that has support for 4.0.

#### Schematron

- SchXslt 1.9.5 replaces the skeleton implementation because the latter is no longer maintained. **Compatibility note:** Some XSpec tests might produce different results with SchXslt.
- XSpec scenarios can verify the text of messages or diagnostics. Add expected text inside `x:expect-assert` or `x:expect-report`.

Many thanks to all the XSpec contributors who made this release possible!  They are listed in the [release notes](https://github.com/xspec/xspec/releases/tag/v3.0.3).
