# Release Manifest

Centralized version registry for COS (Cathodic Operations System) projects.

## Purpose

This repository holds version information files for all COS projects. Each file contains the current release version in CSV format, which is used by VBA applications to check for updates.

## Version File Format

```
version,date,notes,filename
```

Example:
```
1.0.1,2025 July 15,"Bug fixes and improvements",Project Name - 1.0.1.xlsm
```

## Projects Tracked

| File | Project |
|------|---------|
| `cp_version.txt` | Cathodic Protection Rectifier Readings |
| `air_to_soil_version.txt` | Air to Soil |

## Usage

VBA applications check this repository for version updates:
```
https://raw.githubusercontent.com/Antoniofiliona/Release_Manifest/main/<project>_version.txt
```

## Deployment

Version files are automatically updated by the COS Deployment Manager when new releases are deployed to production.
