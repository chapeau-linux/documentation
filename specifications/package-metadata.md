# Package Metadata

## Purpose

This document defines the package metadata required by the Chapeau Linux package format.

Package metadata provides the information necessary to identify, verify, and manage software packages.

Every `.cpkg` package shall contain package metadata conforming to this specification.

## Required Fields

Every package shall define the following metadata fields.

| Field | Description |
| ------ | ----------- |
| Name | A unique identifier for the package. |
| Version | The upstream software version. |
| Release | The package revision for the specified version. |
| Architecture | The target system architecture. |

## Optional Fields

Packages may define additional metadata.

Examples include, but are not limited to:

| Field | Description |
| ------ | ----------- |
| Summary | A concise description of the package. |
| Description | A detailed description of the package. |
| License | The software license. |
| Homepage | The project's website. |
| Maintainer | The package maintainer. |
| Dependencies | Runtime package dependencies. |
| Build Dependencies | Dependencies required to build the package. |
| Optional Dependencies | Packages providing optional functionality. |
| Conflicts | Packages that cannot be installed simultaneously. |
| Replaces | Packages superseded by this package. |
| Provides | Virtual packages or capabilities provided by the package. |

Additional metadata fields may be defined by future specifications.

## Encoding

The encoding and representation of package metadata are defined by their respective specifications.

## Compatibility

Future revisions of this specification may introduce additional metadata fields.

Existing required fields shall remain backward compatible whenever practical.
