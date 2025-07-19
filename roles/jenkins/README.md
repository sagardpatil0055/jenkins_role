# Jenkins Ansible Role

This role installs Jenkins on a Debian/Ubuntu-based system with OpenJDK 21, using the official Jenkins apt repository and GPG key.

## Variables

| Name                 | Default         | Description                      |
|----------------------|------------------|----------------------------------|
| `jenkins_java_package` | `openjdk-21-jdk` | Java version for Jenkins         |

## Usage

```yaml
- hosts: _jenkins
  become: yes
  roles:
    - jenkins
```
