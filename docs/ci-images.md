---
meta:
  - name: description
    content: "Fairwinds rok8s Scripts | Documentation on CI Images"
---
## CI Images

Each new release of rok8s-scripts generates CI images for common workflows. These images include a set of common CI/CD dependencies, including Docker, Kubernetes, Helm, AWS, and Google Cloud client libraries. Starting with these images as a base for deployment workflows ensures that you don't need to spend any build time installing extra dependencies.

We currently include CI Images based on Alpine and Debian Buster as our recommended starting points. The latest Debian Buster release can be pulled from `quay.io/reactiveops/ci-images:v13.0-buster`. A full list of image tags is available on our [Quay repository](https://quay.io/repository/reactiveops/ci-images).

**Deprecation Notice** As of v10 and onward, alpine and stretch will be the only available images.

**Deprecation Notice from 2023-04-24** As Stretch is being removed from maintenance from Debian, we are removing Stretch support from now on.

## Upgrading from v10 to v11

The v11 series of rok8s-scripts will include [Helm 3](https://helm.sh/blog/helm-3-released/). This will require your cluster to be running Helm3 for it to work.

*WARNING* If you deploy your application with Helm3 and it has already been deployed with Helm 2, you may have issues!!! Please [migrate to Helm 3](https://helm.sh/docs/topics/v2_v3_migration/) before using Rok8s-Scripts v11+!!
