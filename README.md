# sample-github-chart-repo

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add chimbu-helm-charts https://chimbuchinnadurai.github.io/sample-github-chart-repo/

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
chimbu-helm-charts` to see the charts.

To generate templates:

    helm template chimbu-helm-charts/mychart

To install the mychart chart:

    helm install mychart chimbu-helm-charts/mychart

To uninstall the chart:

    helm delete mychart
