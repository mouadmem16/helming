## COPY value file to the current directory
helm show values --repo https://charts.longhorn.io longhorn > longhorn.values

## HELM install
helm install longhorn --repo https://charts.longhorn.io longhorn -n longhorn-system --create-namespace --values longhorn.values --version 1.2.3

## HELM upgrade new version
helm upgrade longhorn --repo https://charts.longhorn.io longhorn -n longhorn-system --values longhorn.values

