This is a Ruwnway fork of https://github.com/kuberenetes-learning-group/fuse-device-plugin.

**What is it?**

This repository builds an image that allows kubernetes pods to access `/dev/fuse`. `/dev/fuse` is necessary for building images within pods, which we (Runway) do using [buildah](https://buildah.io/).

**Why a fork?**

We have created a fork to pin the code at a known version to prevent supply chain security risk, as well as tweak the build process.

**How to build?**

1.  Install [go](https://go.dev/doc/install)
2.  Run `make docker`

**How to deploy?**

1.  Install [go](https://go.dev/doc/install)
2.  Run `make all`. This will build the code & image, and then push the image to our repository `927236916793.dkr.ecr.us-east-1.amazonaws.com/runway-fuse-device-plugin`
