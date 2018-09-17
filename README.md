
# An ansible role for installing java

## Oracle java versioning

https://www.oracle.com/technetwork/java/javase/jdk8-naming-2157130.html

i.e.
tar.gz: the file is named jdk-8u181-bla.tar and installs into a directory jdk-1.8.0_181
rpm: the file is named jdk-8u181-linux-x64.rpm, but is registered with name jdk1.8

version number: 8
version: 1.8
full version: 1.8.0
update version number: 181

## Variables

```
java:

  # java version
  version: 8

  # jre or jdk
  type: jre

  # headless or not
  headless: true
```

```
- hosts: all
  roles:
    - role: java/openjdk
```

```
- hosts: all
  roles:
    - role: java/oracle
      java:
        external_archive_file: jre-8u181-linux-x64.rpm
```

```
- hosts: all
  roles:
    - role: java/oracle
      java:
        external_archive_file: jdk-8u181-fcs-bin-b13-linux-arm32-vfp-hflt-07_jul_2018.tar.gz
```
