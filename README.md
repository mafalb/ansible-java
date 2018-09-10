
Variables

java:

  # java version
  version: 8

  # jre or jdk
  type: jre

  # headless or not
  headless: true

- hosts: all
  roles:
    - role: java/openjdk
