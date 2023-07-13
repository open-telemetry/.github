# Security Policy

This security policy applies to all projects under the [open-telemetry organization][gh-organization] on GitHub. Security reports involving specific projects should still be reported following the instructions on this document: the report will be shared by the technical committee to the project leads, who might not all have access to the private key required to decrypt your message.

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

If you are absolutely unable to or have strong reasons not to use GitHub reporting
workflow, please reach out to the maintainers or the Technical Committee using other
[available communication methods](https://opentelemetry.io/community/) and we will
provide instruction on how to report the vulnerability using an encrypted message.

[gh-organization]: https://github.com/open-telemetry
