# Helm Chart Repository

This repository hosts Helm charts via GitHub Pages.

How to use

- Add the repo:
  ```bash
  helm repo add bagetter https://bagetter.github.io/helm-chart-repo
  helm repo update
  ```

- Search for charts:
  ```bash
  helm search repo bagetter
  ```

- Install BaGetter (example):
  ```bash
  helm install my-bagetter bagetter/bagetter --version <chart-version>
  ```

Publishing

- The chart is packaged and published by the CI workflow in the [bagetter/BaGetter](https://github.com/bagetter/BaGetter) repository.
- Packages (.tgz) and `index.yaml` are served from the `gh-pages` branch.
- Ensure `.nojekyll` exists in `gh-pages` so `index.yaml` is served correctly.
