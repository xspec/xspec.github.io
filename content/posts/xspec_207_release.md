---
date: 2020-11-29
linktitle: Release XSpec v2.0.7
title: Release XSpec v2.0.7
weight: 9
categories: [ "Release" ]
tags: ["v2.0.7"]
---

## Release XSpec v2.0.7
Release v2.0.7 introduces new features and enhancements, fixes bugs, and improves the test suite and the documentation. These are the highlights for XSpec v2.0.7:

#### **Common to Languages Under Test**
- [`x:helper`](https://github.com/xspec/xspec/wiki/Integrating-Your-Own-Test-Helpers) lets you integrate your own test helpers
- `@as` can be set in `x:context` and `x:expect`

#### **XSLT**
- You can test XSLT packages and static parameters ([experimental](https://github.com/xspec/xspec/wiki/External-Transformation))

#### **Schematron**
- Compatible with [SchXslt](https://github.com/schxslt/schxslt) (not thoroughly tested)
- You can write advanced expressions in `@location` (e.g. `<x:expect-assert location="//sec[@id='lower']" />`)

#### **XQuery**
- [Text value templates](https://github.com/xspec/xspec/wiki/Text-Value-Templates)
- Arrays and maps are reported in the same way as XSLT scenarios

#### **Command Line**
- New option `-e` treats failed tests as error

#### **Oxygen**
- `${xmlCatalogFilesList}` takes effect in the **Run XSpec Test** transformation scenario

#### **Breaking Changes**
- See https://github.com/xspec/xspec/issues/1121


Many thanks to the many XSpec contributors who made this release possible. They are listed on the [release notes](https://github.com/xspec/xspec/releases/tag/v2.0.7).
