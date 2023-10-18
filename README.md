# Cloud City Crafted Container Images

This repository contains the configuration and scripts needed to create container images for Cloud City Crafted continuous integration (CI) and runtime environments.

## ✨ Quick Start

Ensure you have [Docker](https://docs.docker.com/get-docker/) installed.

> Note: All runner images are compatible with [act](https://github.com/nektos/act) as alternative runner images.

To pull container images, run:

```shell
docker pull ghcr.io/cloud-city-crafted-images/<IMAGE_NAME>:latest
```

And ta-da 🎉! You're ready to run Cloud City Crafted GitHub Actions images locally!

## 📦 Images

| Image                                                                                                                                       | Available Tags     | Included Packages                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| [github-actions-runners-ubuntu](https://github.com/orgs/cloud-city-crafted-images/packages/container/package/github-actions-runners-ubuntu) | `latest`, `v1.0.0` | [GitHub Actions Ubuntu Runner Packages](https://github.com/cloud-city-crafted-images/github-actions-runners-ubuntu/tree/main#-packages) |
| [github-actions-cache](https://github.com/orgs/cloud-city-crafted-images/packages/container/package/github-actions-cache)                   | `latest`, `v1`     | [GitHub Actions Cache Packages](https://github.com/cloud-city-crafted-images/github-actions-cache/tree/main#-packages)                  |

## 🪪 License

This repository is [MIT licensed](./LICENSE).

Base images are subject to their respective open source license(s):

- [Debian](https://www.debian.org/legal/licenses/)

## 📸 Attributions

- Organization Logo is a modified version of [Free Box Icon in Flat Style](https://iconscout.com/free-icon/box-package-parcels-logistic-delivery-packed-shipping-11) by [Mohit Gandhi](https://iconscout.com/contributors/mcgandhi61)
