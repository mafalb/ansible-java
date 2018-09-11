
Variables


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
      external_rpm_file: jre-8u181-linux-x64.rpm
```
