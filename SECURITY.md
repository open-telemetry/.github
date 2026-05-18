# Security Policy

This security policy applies to all projects under the [open-telemetry organization][gh-organization] on GitHub. Security reports involving specific projects should still be reported following the instructions on this document: the report will be shared by the technical committee to the project leads, who might not all have access to the private key required to decrypt your message.

## Security model

<!-- 
    This section is mirrored from the authoritative source at:
    https://github.com/open-telemetry/sig-security/blob/main/security-response.md#supported-versions

    Any changes should be made there first, then synced back here.
-->

When assessing the urgency and importance of a security fix, confidentiality and
integrity are our topmost concerns for all OpenTelemetry software artifacts.

In contrast, we do not consider the default settings of OpenTelemetry software 
artifacts to be secure against availability attacks. We highly recommend not
using insecure defaults where feasible. To ensure availability, users must
require authentication for their endpoint communication following the guidance
on the [Security section of our
website](https://opentelemetry.io/docs/security/).

Additionally, the OpenTelemetry project does not consider the following to be
security vulnerabilities:

- a denial of service attack by properly authenticated clients
- availability-related attack to endpoints by properly authenticated clients

These may still be considered bugs, and users can report them as such. When
assessing availability-related impact, maintainers will also take into account
the security policies of other projects (e.g. Prometheus) when assessing
vulnerabilities against components that provide compatibility with those
projects, as well as the level of asymmetry in terms of resource usage leveraged
by the attack.


## Supported Versions

The OpenTelemetry project provides community support only for the last minor version: bug fixes are released either as part of the next minor version or as an on-demand patch version. Independent of which version is next, all patch versions are cumulative, meaning that they represent the state of our `main` branch at the moment of the release. For instance, if the latest version is 0.10.0, bug fixes are released either as part of 0.11.0 or 0.10.1.

Security fixes are given priority and might be enough to cause a new version to be released.

## Reporting a Vulnerability

If you find something suspicious and want to report it, we'd really appreciate!

### Ways to report

In order for the vulnerability reports to reach maintainers as soon as possible,
the preferred way is to use the `Report a vulnerability` button on the `Security`
tab in the respective GitHub repository. It creates a private communication channel
between the reporter and the maintainers.

For reporting security issues against the website, please report them at
<https://github.com/open-telemetry/opentelemetry.io/security/advisories>.

If you are absolutely unable to or have strong reasons not to use GitHub reporting
workflow, please reach out to security@opentelemetry.io.

[gh-organization]: https://github.com/open-telemetry
