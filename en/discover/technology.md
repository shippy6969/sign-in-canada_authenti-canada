---
layout: default
ref: discover-technology
title: Technology and Architecture
lang: en
---
# Technology and Architecture

## Technology

The Sign In Canada platform is built on [Gluu Server](https://gluu.org), an open-source identity & access management (IAM) platform.

The platform also leverages several cloud services:

* IaaS: Azure Virtual Machines, Azure Virtual Networks, Azure Traffic Manager
* PaaS/SaaS: Azure Storage, Azure Key Vault, Azure Functions, Azure Monitor (Application Insights, Log Analytics), Azure DevOps, Azure Dev/Test Labs, GitHub

## Architecture

![Overview](images/Overview.svg)

## Components

### Acceptance Framework

Product: Gluu Passport

Gluu Passport is a [Node.JS](https://nodejs.org/en/about/) web application based
on the [Express](https://expressjs.com/) web application framework and the
[Passport.JS](http://www.passportjs.org/) authentication middleware.

As the name implies, This is the "Acceptance" component of the Acceptance
Platform. It integrates with credential providers and trusted identity providers
to accept assurances of credential and identity on behalf of GC relying
parties.

Sign in Canada uses a version of Gluu Passport that has been customized to
support some unique functionality that supports the coexistence with, and
transition from, the older GCCF credential services, in particular:

* It has been customized to support both the preservation and run-time migration
  of user's existing PAIs from the CSP to the Acceptance Platform, so that the
  transition has no impact on end users' enrolment with existing relying parties.
* It has customized to support session coordination between the Acceptance
  Platform and the CSPs.

Version: 5.3

Website: https://www.gluu.org/

Source code: https://github.com/sign-in-canada/gluu-passport/

### OpenID Provider

Product: oxAuth

oxAuth is an open source [OpenID Connect](https://openid.net/connect/) Provider
(OP) and [UMA](https://kantarainitiative.org/confluence/display/uma/Home)
Authorization Server (AS).

oxAuth is the core component of the Acceptance Platform, responsible for the
user interface and business logic. As an [OpenID
Connect](https://openid.net/connect/) Provider, it also provides the application
programming interface used by GC relying parties that integrate using [OpenID
Connect](https://openid.net/connect/).

Version: 4.4.0

Website: https://www.gluu.org/

Source code: https://github.com/GluuFederation/oxAuth/

### SAML Identity Provider

Product: Shibboleth IDP

Shibboleth is a [SAML](https://wiki.oasis-open.org/security/FrontPage) Identity
Provider (IDP) that provides the application programming interface used by GC
relying parties that integrate using [SAML](https://wiki.oasis-open.org/security/FrontPage).

Version: 4.4.0

Website: https://www.shibboleth.net/products/identity-provider/

Source code: https://wiki.shibboleth.net/confluence/display/DEV/Source+Code+Access/

### NoSQL Database

Product: Couchbase Enterprise Server

Couchbase Server is an open-source, distributed, multi-model NoSQL
document-oriented database software package that is optimized for interactive
applications.

The Sign In Canada platform uses Couchbase to store user profiles and relying
party configurations, as well as for high-performance distributed session
caching.

Version: 6.6.5

Website: https://www.couchbase.com/
