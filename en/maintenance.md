---
layout: default
ref: maintenance
title: Upcoming Planned Maintenance
lang: en
---
# Upcoming Planned Maintenance

## Friday May 27, 2022 7:00AM EDT

### Environments Affected

* Client Acceptance Test

### Description

The Sign In Canada team will be updating the cryptographic keys used to
authenticate to the GCKey and CBS Test Environments between 7AM and 8AM eastern
time on Friday May 27.
 
In order to maintain integration between the Sign In Canada Client Acceptance
Test Environment (CATE) and the two SSC credential services, 2Keys and SecureKey
will need to configure these new keys simultaneously. These
changes are being closely coordinated between TBS, SSC and both vendors in order
to minimize downtime, however clients may briefly encounter errors while the
change is underway.
 
The scope of this change is limited to the Acceptance Test
Environment (CATE). The production environment will not be impacted.

## Friday May 27, 2022 9:00PM EDT

### Environments Affected

* Client Acceptance Test

### Description

The Sign In Canada team will be deploying a new release of the Sign In Canada platform
[Release 1.2.98](https://github.com/sign-in-canada/Acceptance-Platform/releases/tag/v1.2.98)
to the client acceptance test environment. The installation is scheduled for 9PM
and is expected to result in an outage of approximately 35 minutes.

## Sunday May 29, 2022 4:00AM EDT

### Environments Affected

* Production

### Description

The latest Linux security patches will be applied to the production environment
starting at 4AM. This will result in an outage of approximately 12 minutes.

