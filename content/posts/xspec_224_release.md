---
date: 2021-10-08
linktitle: Release XSpec v2.2.4
title: Release XSpec v2.2.4
weight: 7
categories: [ "Release" ]
tags: ["v2.2.4"]
---

## Release XSpec v2.2.4
Release v2.2.4 introduces new features and enhancements, fixes bugs, and improves the test suite and the documentation. These are the highlights for XSpec v2.2.4:

#### Common to Languages Under Test

- Pending or unfocused variable declarations are handled more gracefully.
- Large results are no longer saved in separate XML files by default.
- This will be the last version to support Saxon 9.8.

#### XSLT

- Multiple test scenarios can be run in parallel by setting `@threads` on `x:description` or `x:scenario`. (Requires Saxon-EE)
- You can set `x:context` when testing functions. (Requires `/x:description/@run-as`=`external`)

#### Schematron

- You can mark assertions as pending by setting `@pending` on `x:expect-*` elements, as an alternative to using the `x:pending` element.
- When `@location` does not point to one node, the error message is more helpful.

Many thanks to the many XSpec contributors who made this release possible. They are listed on the [release notes](https://github.com/xspec/xspec/releases/tag/v2.2.4).
