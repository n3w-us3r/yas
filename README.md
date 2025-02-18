# YAS: Yet Another Shop

YAS is a pet project aim to practice building a typical microservice application in Java

[![storefront-ci](https://github.com/nashtech-garage/yas/actions/workflows/storefront-ci.yaml/badge.svg)](https://github.com/nashtech-garage/yas/actions/workflows/storefront-ci.yaml)
[![storefront-bff-ci](https://github.com/nashtech-garage/yas/actions/workflows/storefront-bff-ci.yaml/badge.svg)](https://github.com/nashtech-garage/yas/actions/workflows/storefront-bff-ci.yaml)
[![backoffice-ci](https://github.com/nashtech-garage/yas/actions/workflows/backoffice-ci.yaml/badge.svg)](https://github.com/nashtech-garage/yas/actions/workflows/backoffice-ci.yaml)
[![backoffice-bff-ci](https://github.com/nashtech-garage/yas/actions/workflows/backoffice-bff-ci.yaml/badge.svg)](https://github.com/nashtech-garage/yas/actions/workflows/backoffice-bff-ci.yaml)
[![product-ci](https://github.com/nashtech-garage/yas/actions/workflows/product-ci.yaml/badge.svg)](https://github.com/nashtech-garage/yas/actions/workflows/product-ci.yaml)
[![media-ci](https://github.com/nashtech-garage/yas/actions/workflows/media-ci.yaml/badge.svg)](https://github.com/nashtech-garage/yas/actions/workflows/media-ci.yaml)
[![cart-ci](https://github.com/nashtech-garage/yas/actions/workflows/cart-ci.yaml/badge.svg)](https://github.com/nashtech-garage/yas/actions/workflows/cart-ci.yaml)
[![customer-ci](https://github.com/nashtech-garage/yas/actions/workflows/customer-ci.yaml/badge.svg)](https://github.com/nashtech-garage/yas/actions/workflows/customer-ci.yaml)

## Tentative technologies and frameworks

- Java 17
- Spring boot 2.7
- Next.js
- Keycloak
- Kafka
- K8s
- Github Actions
- SonarCloud
- OpenTelemetry
- Grafana, Loki, Prometheus, Tempo

## Local development architecture

![Yas - local development architecture](https://raw.githubusercontent.com/nashtech-garage/yas/main/yas_architecture_local.png)

## Getting started with Docker Compose

1. Get the latest source code
1. Add the following records to your host file: 
`
127.0.0.1 identity
127.0.0.1 api.yas.local
127.0.0.1 pgadmin.yas.local
127.0.0.1 storefront
127.0.0.1 backoffice
127.0.0.1 loki
127.0.0.1 tempo
127.0.0.1 grafana
`
1. Open terminal of your choice, go to 'yas' directory and run `docker compose up`
1. Open your favorite browser and go to  http://pgadmin.yas.local. Account login: admin@yas.com / admin. Register a server: postgres, port 5432, username admin, password admin
1. [Setup Keycloak](https://github.com/nashtech-garage/yas/wiki/Keycloak-Setup/)
1. The Postgresql server is also published to the host machine: servername: localhost, port: 5432, username: admin, password: admin

## Components roadmap
- [x] Identity service
- [x] Media service
- [ ] Product service
- [ ] Pricing service
- [ ] Cart service
- [ ] Order service
- [ ] Review service

## Contributing
- Give us a star
- Reporting a bug
- Participate discussions
- Propose new features
- Submit pull requests. If you new to GitHub, consider to [learn how to contribute to a project through forking](https://docs.github.com/en/get-started/quickstart/contributing-to-projects)

By contributing, you agree that your contributions will be licensed under MIT License. 

Active contributors might be asked to join the core team
