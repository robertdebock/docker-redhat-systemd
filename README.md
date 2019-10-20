Docker RedHat Systemd
=====================

This Dockerfile can build containers capable to use systemd.

Branches
--------

This repository has multiple branches that relate to RedHat versions.

|Branch |RedHat Version|Docker image tag|
|-------|--------------|----------------|
|master |latest (8)    |latest          |
|7      |7             |7               |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  robertdebock/docker-redhat-systemd
```
