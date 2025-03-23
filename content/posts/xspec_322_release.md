---
date: 2025-03-24
linktitle: Release XSpec v3.2.2
title: Release XSpec v3.2.2
weight: 6
categories: ["Release"]
tags: ["v3.2.2"]
---

<a href="https://github.com/xspec/xspec/issues/1766"><img align="right" src="https://user-images.githubusercontent.com/10128303/262700963-1a1e0fda-f335-4c90-9f8a-f72c5ece6c27.png" width="100px" alt="XSpec logo proposed and discussed in #1766"/>
</a>

## Release XSpec v3.2.2

XSpec 3.2 enhances its HTML reports with coverage statistics and a choice of color themes. These are the highlights of XSpec v3.2:

## Common to Languages Under Test

- Test reports use black text on white background by default, improving accessibility. Themes `'whiteblack'` (white on black) and `'classic'` (earlier green/pink design) are also available. You can select a non-default theme using the `xspec.html.report.theme` Ant property or, in the command line interface, the `XSPEC_HTML_REPORT_THEME` environment variable.

## XSLT

- Code coverage report includes a Contents section with coverage statistics and navigation links to module-specific sections of the report.

## XQuery
- XSpec is tested with BaseX 11.8.

## Schematron
- Tests for Schematron can verify string values of Schematron properties.

Many thanks to all the XSpec contributors who made this release possible! They are listed in the [release notes](https://github.com/xspec/xspec/releases/tag/v3.2.2).
