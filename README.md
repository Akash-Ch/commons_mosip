[![Codacy Badge](https://api.codacy.com/project/badge/Grade/8d3ac22fb06f4652bed3d9552db51dc4)](https://app.codacy.com/gh/Akash-Ch/commons_mosip?utm_source=github.com&utm_medium=referral&utm_content=Akash-Ch/commons_mosip&utm_campaign=Badge_Grade_Settings)
[![Maven Package upon a push](https://github.com/mosip/commons/actions/workflows/push_trigger.yml/badge.svg?branch=release-1.2.0.1)](https://github.com/mosip/commons/actions/workflows/push_trigger.yml)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=mosip_commons&metric=alert_status)](https://sonarcloud.io/dashboard?branch=release-1.2.0.1&id=mosip_commons)


# Commons

## Overview
As the name suggests, Commons refers to all the common services (also called "kernel") that are used by other modules of MOSIP. The Kernel services are listed below:

## Databases
Refer to [SQL scripts](db_scripts).

## Build & run (for developers)
The project requires JDK 1.11. 
1. Build and install:
    ```
    $ cd kernel
    $ mvn install -DskipTests=true -Dmaven.javadoc.skip=true -Dgpg.skip=true
    ```
1. Build Docker for a service:
    ```
    $ cd <service folder>
    $ docker build -f Dockerfile
    ```

## Deploy
To deploy Commons services on Kubernetes cluster using Dockers refer to [Sandbox Deployment](https://docs.mosip.io/1.2.0/deployment/sandbox-deployment).

## Test
Automated functaionl tests available in [Functional Tests repo](https://github.com/mosip/mosip-functional-tests).

## APIs
API documentation is available [here](https://mosip.github.io/documentation/).

## License
This project is licensed under the terms of [Mozilla Public License 2.0](LICENSE).


