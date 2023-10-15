# Cloud City Crafted Images

Cloud City Crafted stores container images via [GitHub Packages](https://docs.github.com/en/packages/learn-github-packages/introduction-to-github-packages) under the @cloud-city-crafted-images.

## ✨ Quick Start

Ensure you have [Docker](https://docs.docker.com/get-docker/) installed.

To pull available container images, run:

```shell
docker pull ghcr.io/cloud-city-crafted-images/<IMAGE_NAME>:latest
```

And ta-da 🎉! You're ready to use Cloud City Crafted container images locally!

## 📦 Available Images

| Image                                                                                                                                       | Available Tags | Included Packages                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| [github-actions-cache](https://github.com/orgs/cloud-city-crafted-images/packages/container/package/github-actions-cache)                   | `latest`, `v1` | [GitHub Actions Cache Packages](https://github.com/cloud-city-crafted-images/github-actions-cache#-packages)                   |
| [github-actions-runners-ubuntu](https://github.com/orgs/cloud-city-crafted-images/packages/container/package/github-actions-runners-ubuntu) | `latest`, `v1` | [GitHub Actions Runners Ubuntu Packages](https://github.com/cloud-city-crafted-images/github-actions-runners-ubuntu#-packages) |

## 🛠️ Building Images

To build an image, run:

```shell
docker build \
    --platform linux/amd64 \
    --tag <IMAGE_NAME>:latest \
    --tag ghcr.io/cloud-city-crafted-images/<IMAGE_NAME>:latest \
    --tag <IMAGE_NAME>:<VERSION_TAG> \
    --tag ghcr.io/cloud-city-crafted-images/<IMAGE_NAME>:<VERSION_TAG> \
    ./<ACTION_NAME>
```

where:

- `<IMAGE_NAME>`: Name of the image (e.g., `github-actions-cache`)
- `<VERSION_TAG>`: Major version of the image (e.g., `v1`)

For example, to build the `v1` version of the cache action, use:

```shell
docker build \
    --platform linux/amd64 \
    --tag github-actions-cache:latest \
    --tag ghcr.io/cloud-city-crafted-images/github-actions-cache:latest \
    --tag github-actions-cache:v1 \
    --tag ghcr.io/cloud-city-crafted-images/github-actions-cache:v1 \
    .
```

## 🚀 Deploying Images

To deploy an image to the GitHub Container Registry, use:

```shell
docker push --all-tags ghcr.io/cloud-city-crafted-images/<IMAGE_NAME>
```

where:

- `<IMAGE_NAME>`: Name of the image (e.g., `github-actions-cache`)

For example, to push all github-action-cache images, use:

```shell
docker push --all-tags ghcr.io/cloud-city-crafted-images/github-actions-cache
```

## 🪪 License

The repositories in this organization are [MIT licensed](./LICENSE). See individual repositories for more details.
