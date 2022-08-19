# helm-charts

Helm charts published by datacoves

## How to add a new helm chart?

1. Add git submodule under `repos`
2. Create a symlink under `helm` to the right folder

## How to publish a new release?

1. Bump version on `CR_RELEASE_NAME_TEMPLATE` in `.github/workflows/helm-release.yml`
2. Bump helm chart version (`chart.yaml`)
3. Retrieve latest changes on git submodules

## Helm charts in this repo

(Index)[https://datacoves.github.io/helm-charts/index.yaml]

### Airflow

```
helm repo add datacoves https://datacoves.github.io/helm-charts
helm repo update
helm install datacoves/airflow
```
