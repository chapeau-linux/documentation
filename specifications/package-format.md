# Package Format

## Purpose

This document defines the Chapeau Linux package format (`.cpkg`).

The package format provides a standardized method for distributing software throughout the Chapeau Linux ecosystem.

## Overview

A Chapeau package is a Zstandard-compressed tar archive using the `.cpkg` file extension.

A package contains the information required to install, verify, and manage software on a Chapeau Linux system.

## File Extension

Packages shall use the `.cpkg` file extension.

Example:

```text
package-name-version-release.architecture.cpkg
```

## Archive Format

A `.cpkg` package shall:

- Use the POSIX tar archive format.
- Be compressed using Zstandard (`zstd`).
- Preserve file permissions, symbolic links, and other filesystem metadata where applicable.

## Package Contents

A package may contain:

- Package metadata
- Files to be installed
- Installation or removal scripts
- Integrity information
- Digital signatures

The organization and representation of these components are defined by their respective specifications.

## Package Metadata

Every package shall contain metadata describing the package.

The metadata shall include, at minimum:

- Package name
- Version
- Release
- Target architecture

Additional metadata is defined separately.

## Integrity

Packages shall include integrity information allowing corruption to be detected before installation.

## Authenticity

Official packages shall be digitally signed.

Package managers shall verify package signatures before installation.

## Compatibility

Changes to the package format shall preserve backward compatibility whenever practical.

Breaking changes require a new package format revision.
