# postfixadmin-fetchmail-charts

[![Build Status](https://drone.cryptic.systems/api/badges/volker.raschek/postfixadmin-fetchmail-charts/status.svg)](https://drone.cryptic.systems/volker.raschek/postfixadmin-fetchmail-charts)
[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/volker-raschek)](https://artifacthub.io/packages/search?repo=volker-raschek)

This helm chart contains the cron job deployment of the fetchmail job
from the [postfixadmin](https://github.com/postfixadmin/postfixadmin) project.
The backend database provided by postfixadmin is required. Checkout the [helm
chart](https://github.com/volker-raschek/postfixadmin-charts) for postfixadmin
to deploy the application on kubernetes.

Alternatively can also the database backend of an external postfixadmin
installtion be used. Exactly for this reason is the cron job of fetchmail
independent of the postfixadmin chart.

This helm chart can be found on [artifacthub.io](https://artifacthub.io/) and
can be installed via helm.

```bash
helm repo add volker.raschek https://charts.cryptic.systems/volker.raschek
helm install postfixadmin-fetchmail volker.raschek/postfixadmin-fetchmail
```

## Customization

All [configuration
options](https://github.com/volker-raschek/postfixadmin-fetchmail-docker#environment-variables)
can be defined in the `values.yml` file below the `config` section.
Alternatively can be the options passed via the `--set` flag of the `helm
install` command.
