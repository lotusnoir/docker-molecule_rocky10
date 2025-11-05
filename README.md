# Docker Image with rocky10 base image

This repo was created in order to test ansible roles with molecule.

## Build it locally

  docker build -t rocky10img .
  docker run -d -name rocky10con --cgroupns=host --volume=/sys/fs/cgroup:/sys/fs/cgroup:rw rocky10img
  docker exec -it rocky10con bash


## Use it from dockerhub

    https://hub.docker.com/repository/docker/lotusnoir/ansible_molecule_test_images:rocky10
