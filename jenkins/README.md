## COPY value file to the current directory
helm show values --repo https://charts.jenkins.io jenkins > jenkins.values

## HELM install
helm install jenkins --repo https://charts.jenkins.io jenkins -n jenkins --create-namespace --values jenkins.values

## HELM upgrade new version
helm upgrade jenkins --repo https://charts.jenkins.io jenkins -n jenkins --values jenkins.values


