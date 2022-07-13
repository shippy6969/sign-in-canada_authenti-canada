---
layout: default
ref: maintenance
title: Upcoming Planned Maintenance
lang: en
---
# Upcoming Planned Maintenance

## Thursday July 14, 2022 9:00PM EDT

### Environments Affected

* Client Acceptance Test

### Description

The Sign In Canada team will be deploying a new release of the Sign In Canada platform
[Release 1.2.132](https://github.com/sign-in-canada/Acceptance-Platform/releases/tag/v1.2.132)
to the to the client acceptance test environment. The installation is scheduled for 9PM
and is expected to result in an outage of approximately 40 minutes.

## Tuesday July 19, 2022 7:00AM EDT

### Environments Affected

* Production

### Description

Shared Services Canada will be updating the cryptographic keys used by the GCKey
and CBS Production Environments between 7AM and 8AM.

In order to maintain integration between the Sign In Canada Production
Environment and the two SSC credential services, the Sign In Canada team will
need to configure these new keys during this same time window. These changes are
being closely coordinated between TBS and SSC in order to minimize downtime,
however users may briefly encounter errors while the change is underway.

## Sunday July 24, 2022 4:00AM EDT

### Environments Affected

* Production

### Description

If no issues are identified during client acceptance testing of [Release
1.2.132](https://github.com/sign-in-canada/Acceptance-Platform/releases/tag/v1.2.132),
then the Sign In Canada team plans to promote this release to production on July 24.
The installation is scheduled for 4AM and is expected to result in an outage
of approximately 40 minutes.
