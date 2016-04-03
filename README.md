# Wercker Kubuernetes Talk #

These are the files for the Wercker + Kubernetes Talk

## Intention ##

The goal of this talk/files is to give a complete example how a workflow with
wercker and kubernetes could work with multiple microservices.

All files are built for Kubernetes 1.2.0.

## General things ##
Everything that shares the same codebase is seen as a microservice.
A microserice can have other services like mysql, rabbitmq or redis that dont have a repo.




## Architecture ##

The goal is to spin up the following microservices:

#### kubernetes core resources ####
[wercker-k8s-talk-kubernetes-core-resources](https://github.com/stvnwrgs/wercker-k8s-talk-kubernetes-core-resources)

#### guestbook ####
[wercker-k8s-talk-guestbook](https://github.com/stvnwrgs/wercker-k8s-talk-guestbook)
1. the go application for the guestbook
2. redis-master
3. redis-slave

#### emitter ####
[wercker-k8s-talk-emitter](https://github.com/stvnwrgs/wercker-k8s-talk-emitter)

#### persister ####
[wercker-k8s-talk-persister](https://github.com/stvnwrgs/wercker-k8s-talk-persister)