# Dockerfile Collections for the GitLab Local Runners
[![Debian10](https://github.com/jeonghanlee/Dockerfiles/actions/workflows/debian10.yml/badge.svg)](https://github.com/jeonghanlee/Dockerfiles/actions/workflows/debian10.yml)
[![Rocky8](https://github.com/jeonghanlee/Dockerfiles/actions/workflows/rocky8.yml/badge.svg)](https://github.com/jeonghanlee/Dockerfiles/actions/workflows/rocky8.yml)
[![CentOS7](https://github.com/jeonghanlee/Dockerfiles/actions/workflows/centos7.yml/badge.svg)](https://github.com/jeonghanlee/Dockerfiles/actions/workflows/centos7.yml)

For saving valuable resouces (time, electricity, computing power, and so on), this collections will be used to generate Linux Images with the EPICS environment with full libraries for the gitlab runner. The image size is still big. However, these images should contains almost all libraries for the EPICS application.

The following example commands are good for building its docker image locally. The all docker images are built through the Github Actions.

## Debian 10 + EPICS

```bash
bash docker_builder.bash -t debian10
```

## Rocky 8 + EPICS

```bash
bash docker_builder.bash -t rocky8
```

## CentOS7 + EPICS

```bash
bash docker_builder.bash -t centos7
```

## The EPICS environment and others

The EPICS environment is done by default. And one can find `/usr/local/epics/` path. The additional application(s) (for example, `pmd`) will be installed in `/usr/local/apps` path. Its configuration `.bashrc` is located in `/root/.bashrc`.


