# searchparty/polymer-firebase-docker

## Purpose

This image was created specifically for usage with continuous integration systems. It contains the requirements to build a project with [Polymer](https://www.polymer-project.org/) and deploy project to [Firebase](https://firebase.google.com/)

Adapted from [devillexio/docker-firebase](https://github.com/devillexio/docker-firebase)

Available on [Docker Hub](https://hub.docker.com/r/searchparty/polymer-firebase-bower/)

## Build

```
docker build --tag searchparty/polymer-firebase-bower .
```

## Details

### Base Image

* [node (boron)](https://hub.docker.com/r/library/node/) - The latest Node LTS (Boron) image

### Additional Node Modules

* [Polymer CLI](https://www.polymer-project.org/2.0/docs/tools/polymer-cli) - Polymer CLI is a command-line interface for Polymer projects. Required to build Polymer.

* [Firebase CLI](https://github.com/firebase/firebase-tools) - Firebase Command Line Tools. Required to deploy to Firebase.

* [Bower](https://bower.io/) - Bower for package management