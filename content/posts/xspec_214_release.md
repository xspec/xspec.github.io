---
date: 2021-04-30
linktitle: Release XSpec v2.1.4
title: Release XSpec v2.1.4
weight: 8
categories: [ "Release" ]
tags: ["v2.1.4"]
---

## Release XSpec v2.1.4
Release v2.1.4 introduces new features and enhancements, fixes bugs, and improves the test suite and the documentation. These are the highlights for XSpec v2.1.4:

#### **Common to Languages Under Test**
- You can mark assertions as pending by setting `@pending` on `x:expect`, as an alternative to using the `x:pending` element.
- `/x:description/@measure-time` measures elapsed run times of scenarios. (Requires Saxon-PE or EE.)

#### **XSLT**
- Different scenarios can use different global parameters (`//x:scenario/x:param`). (Requires [`/x:description/@run-as="external"`](https://github.com/xspec/xspec/wiki/External-Transformation).)

#### **Schematron**
- Fully tested with [SchXslt](https://github.com/schxslt/schxslt) v1.7.1
- Supports [`/x:description/@run-as`](https://github.com/xspec/xspec/wiki/External-Transformation)

Many thanks to the many XSpec contributors who made this release possible. They are listed on the [release notes](https://github.com/xspec/xspec/releases/tag/v2.1.4).
