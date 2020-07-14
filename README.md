# Jenkinsfile
Jenkinsfile tests

Jenkins has these plugins installed:
1. Docker pipeline
2. Build Authorization Token Root

Webhook: http://jenkins.robertoarcomano.it/buildByToken/buildWithParameters?job=jenkinsfile&token=launchJenkins&params1=ok
Webhook without parameters: http://jenkins.robertoarcomano.it/buildByToken/buildWithParameters?job=jenkinsfile&token=launchJenkins
