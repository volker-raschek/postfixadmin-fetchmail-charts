# postfixadmin-fetchmail-charts

[![Build Status](https://postfixadmin-fetchmail.cryptic.systems/api/badges/volker.raschek/postfixadmin-fetchmail-runner-charts/status.svg)](https://postfixadmin-fetchmail.cryptic.systems/volker.raschek/postfixadmin-fetchmail-runner-charts)
[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/volker-raschek)](https://artifacthub.io/packages/search?repo=volker-raschek)

This is helm chart is an addon for
[postfixadmin-fetchmail-runner](https://github.com/postfixadmin-fetchmail/postfixadmin-fetchmail-runner-kube)
and should replace the official unmainted helm chart
[repository](https://github.com/postfixadmin-fetchmail/postfixadmin-fetchmail-runner-kube).

This helm chart can be found on [artifacthub.io](https://artifacthub.io/) and
can be installed via helm.

```bash
helm repo add volker.raschek https://charts.cryptic.systems/volker.raschek
helm install postfixadmin-fetchmail volker.raschek/postfixadmin-fetchmail-runner
```

## Customization

All [configuration
options](https://github.com/volker-raschek/postfixadmin-fetchmail-docker#supported-environment-variables)
can be defined in the `values.yml` file below the `config` section.
Alternatively can be the options passed via the `--set` flag of the `helm
install` command.
