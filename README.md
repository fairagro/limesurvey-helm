# Kubernetes Helm Charts

## Add Helm Repository

```
helm repo add limesurvey https://fairagro.github.io/limesurvey-helm/
helm repo update
```

# Helm Charts

The following Helm Charts are available:

* [LimeSurvey](./limesurvey/README.md)

# On this repo #

This is a fork of https://github.com/martialblog/helm-charts which provides a helm chart for limesurvey (and for ejabberd). We've forked this repo to add some missing features. The chart is published using github pages. To create a new chart release, go to the folder where you've cloned this repo and execute these commands:

```bash
helm package limesurvey
helm repo index . --url https://github.com/fairagro/limesurvey-helm
```

The first command will create the package file `limesurvey-<x.z.y>.tgz` and the second one will create the index file `index.yaml`. Both need to be commited to the repo.