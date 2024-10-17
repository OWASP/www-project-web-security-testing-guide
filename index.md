---
layout: col-sidebar
title: OWASP Web Security Testing Guide
tags: otg wstg
level: 4
type: documentation
pitch: The Web Security Testing Guide (WSTG) Project produces the premier cybersecurity testing resource for web application developers and security professionals.
---

[![OWASP Flagship](https://img.shields.io/badge/owasp-flagship-brightgreen.svg)](https://owasp.org/projects/#all-projects)
[![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/)
[![WSTG Github Stars](https://img.shields.io/github/stars/OWASP/wstg?label=Stars%20on%20GitHub&style=social)](https://github.com/OWASP/wstg/)
[![Twitter Follow](https://img.shields.io/twitter/follow/owasp_wstg?style=social)](https://twitter.com/owasp_wstg)

The Web Security Testing Guide (WSTG) Project produces the premier cybersecurity testing resource for web application developers and security professionals.

The WSTG is a comprehensive guide to testing the security of web applications and web services. Created by the collaborative efforts of cybersecurity professionals and dedicated volunteers, the WSTG provides a framework of best practices used by penetration testers and organizations all over the world.

## Contributions

Any contributions to the guide itself should be made via the [guide's project repo](https://github.com/OWASP/wstg).

:stop_sign: Contributions should only be made in the proper repo against the latest content. Please don't open PRs here for versioned or stable content, they represent point-in-time state.  

## Stable

View the always-current stable version at [stable](stable/).

## Latest

We are currently developing release version 5.0.

You can [read the latest development documents in our official GitHub repository](https://github.com/OWASP/wstg/tree/master/document) or view the bleeding-edge content at [latest](latest/).

## Versioned Releases

[v4.2](v42/) is currently available as a web-hosted release and PDF. Previous releases are available as PDFs and in some cases web content via the **Release Versions** tab.

## How To Reference WSTG Scenarios

Each scenario has an identifier in the format `WSTG-<category>-<number>`, where: 'category' is a 4 character upper case string that identifies the type of test or weakness, and 'number' is a zero-padded numeric value from 01 to 99. For example:`WSTG-INFO-02` is the second Information Gathering test.

The identifiers may change between versions therefore it is preferable that other documents, reports, or tools use the format: `WSTG-<version>-<category>-<number>`, where: 'version' is the version tag with punctuation removed. For example: `WSTG-v41-INFO-02` would be understood to mean specifically the second Information Gathering test from version 4.1.

If identifiers are used without including the `<version>` element then they should be assumed to refer to the latest Web Security Testing Guide content. Obviously as the guide grows and changes this becomes problematic, which is why writers or developers should include the version element.

### Linking

Linking to Web Security Testing Guide scenarios should be done using versioned links not `stable` or `latest` which will definitely change with time. However, it is the project team's intention that versioned links not change. For example: `https://owasp.org/www-project-web-security-testing-guide/v42/4-Web_Application_Security_Testing/01-Information_Gathering/02-Fingerprint_Web_Server`. Note: the `v42` element refers to version 4.2.
