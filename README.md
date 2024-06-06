# Greenplum DB 6 - Open Source Version EL9 - Unofficial RPMs

## **IT IS NOT AN OFFICIAL GREENPLUM DB RELEASE - IT'S A RECOMPILED VERSION**

If you are here, you are looking for the latest Greenplum DB version 6 RPMs for
EL9. As you probably know, the official project was archived, and its future is
uncertain.


The repository contains GPDB version `6-6.27.1`, the latest tag/version
available. It's our own recompilation with some build patches, so it's not the
official Greenplum DB release for Enterprise Linux 9.


One of the most important changes is the addition of the `--enable-gpperfmon` to
the build process. Also, everything was packed in RPMs.


**These packages probably won't be developed further and are provided as is. As
long as there is no clear and definite decision about the future of GPDB and
its open-sourced version, we are unable to say if it will ever be updated.**


## Installation

Installation is as simple as downloading the packages and installing them.

```bash
mkdir gpdb-packages
# Get only these packages you need or all of them
wget -P gpdb-packages https://github.com/SourceMation/gpdb-6-el9-rpms/releases/download/6-6.27.1/diskquota-2.3.0-1.el9.x86_64.rpm
wget -P gpdb-packages https://github.com/SourceMation/gpdb-6-el9-rpms/releases/download/6-6.27.1/gpbackup-1.0.0-1.el9.x86_64.rpm
wget -P gpdb-packages https://github.com/SourceMation/gpdb-6-el9-rpms/releases/download/6-6.27.1/gpbackup-s3-plugin-1.0.0-1.el9.x86_64.rpm
wget -P gpdb-packages https://github.com/SourceMation/gpdb-6-el9-rpms/releases/download/6-6.27.1/gpupgrade-1.0.0-1.el9.x86_64.rpm
wget -P gpdb-packages https://github.com/SourceMation/gpdb-6-el9-rpms/releases/download/6-6.27.1/open-source-greenplum-db-6.27.1-rhel9-x86_64.rpm
wget -P gpdb-packages https://github.com/SourceMation/gpdb-6-el9-rpms/releases/download/6-6.27.1/pgbouncer-gp-1.0.0-1.el9.x86_64.rpm
wget -P gpdb-packages https://github.com/SourceMation/gpdb-6-el9-rpms/releases/download/6-6.27.1/pxf-gp6-6.10.1-SNAPSHOT.el9.x86_64.rpm
sudo dnf install gpdb-packages/*.rpm
```


## System preparation/start/administarion

Consult the official documentation and remember about things like
`/usr/local/greenplum-db/greenplum_path.sh` etc.


## Migration support

If you are considering migration to another database, buying the commercial
solution, or need assistance with it, we are here to support you. Contact us at
sourcemation at linuxpolska.com. **We are vendor-neutral** and can assist you
with both migration and obtaining official support for commercially enhanced
Greenplum DB (depending on availability).
