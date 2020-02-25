# Sonar-Scanner NodeJS

A sonar-scanner image based on `node:12-buster-slim` for node projects analyzing.  
It has no entrypoint to be used in CircleCI

## Includes:
- openjdk 13
- sonar-scanner 4.2.0.1873
- git

## Usage:
```sh
sonar-scanner \
    -Dsonar.projectKey=<PROJECT_KEY> \
    -Dsonar.projectName=<PROJECT_NAME> \
    -Dsonar.projectSource=<PROJECT_DIR> \
    -Dsonar.projectVersion=<PROJECT_VERSION> \
    -Dsonar.host.url=<SONARQUBE_URL> \
    -Dsonar.login=<SONARQUBE_TOKEN>
```

Documentation: https://docs.sonarqube.org/latest/analysis/scan/sonarscanner/
