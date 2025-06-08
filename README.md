# xosview for AlmaLinux 9

This repository provides RPM and SRPM packages of `xosview` (v1.23) built for AlmaLinux 9.

## Verified on:
- AlmaLinux 9.6
- x86_64 architecture
- Built with `rpmbuild` using custom SPEC file
- Runtime verified under a virtual X display (Xvfb)

## Contributor
- Akiyoshi Kurita

## Purpose
This effort addresses the absence of a lightweight, legacy-friendly system monitor in AlmaLinux 9窶冱 default repositories. It demonstrates:

- Architecture validation on RHEL9-compatible platforms  
- Legacy tool support for production and public-sector environments  
- Transparent, reproducible RPM packaging

## Installation
```bash
sudo dnf install -y ./RPMS/xosview-1.23-2.el9.x86_64.rpm
```

## Build
```bash
dnf install -y libX11-devel libXpm-devel rpm-build
rpmbuild -ba SPECS/xosview.spec
```

## License
This software is distributed under the terms of the GNU GPL v2. See `LICENSE` for details.

