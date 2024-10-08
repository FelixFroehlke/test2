# Software Bill of Materials (SBOM)

## Explanation

```
TODO: You can remove this section upon creating your own repository
```
To secure and validate Leadec's Software Supply Chain, every repository shall list their dependencies, as well as sub- and sub-subdependencies and so forth (those are called collectively `transitive dependencies`).

Many tools exist to automate this and include it in various build systems. See [SPDX on GitHub](https://github.com/spdx) - an ISO standardized, maschine and human readable SBOM format. They provide tooling for many major build systems to automatically create an SPDX document from your compile time dependencies.

However: Many more dependencies exist for a software system apart from compile-time dependencies. Oftentimes listing them cannot be automated. For example: Requirements to the production runtime environment, externally called APIs or subsystems, included images and fotography in the software, etc.

Those need to be listed too.

For open source licenses SPDX Identifier should be used. See [SPDX Codes](https://spdx.org/licenses/).

## Introduction

To secure and validate Leadec's Software Supply Chain, in regards to

- license compliance
- IT supply chain security
- IT security reactions and upgrades
- duediligence, warranty and right to repair
- external dependencies and involved risks
- maintainability, upgradability and stability over time

the following list shall serve as an aid for later maintainers and operations personnel to inspect the (direct and transitive) dependencies of this software.

## Non-automated Listing

| Dependency Name | Include Type       | Version                            | License          | Link to origin               |
|-----------------|--------------------|------------------------------------|------------------|------------------------------|
| LabVIEW         | Runtime Platform   | 2020                               | NATIONAL INSTRUMENTS SOFTWARE LICENSE AGREEMENT | https://www.ni.com/en/about-ni/legal/software-license-agreement.html |

## Redistributed Licenses

Note that some licenses of the compiled dependencies require us to state the encumbered license of these dependencies to the end user.
These statements can be found in the [LICENSES.md](./LICENSES.md)
