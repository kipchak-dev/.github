<div align="center">

<a href="https://kipchak.dev"><img src="./kipchak-banner.svg" alt="Kipchak, an API development kit for PHP" width="100%" /></a>

[**kipchak.dev**](https://kipchak.dev) · [Getting started](https://kipchak.dev/docs/getting-started) · [Packages](https://kipchak.dev/ecosystem) · [Enterprise](https://kipchak.dev/enterprise) · [Journal](https://mamluk.net/journal/) · [llms.txt](https://kipchak.dev/llms.txt)

</div>

---

Kipchak is an API development kit for PHP 8.4 and later. It gives an API the structure of a framework without the
weight of one: [Slim 4](https://www.slimframework.com/) underneath, [FrankenPHP](https://frankenphp.dev/) in worker
mode in front, and independent drivers and middleware for the services an API depends on. Everything an endpoint does
is visible in the project's own code, and the OpenAPI document is generated from it. Kipchak serves 3,000 requests per
second per instance in production on the AlAdhan API.

```bash
composer create-project kipchak/starter my-api
cd my-api
docker compose up --watch
```

The API then answers on `http://localhost:8080/v1/sultans`, and its OpenAPI document is at `/openapi.json`.

## Repositories

These repositories are **read-only mirrors**. Development takes place on [1x.ax](https://1x.ax/mamluk/kipchak), and pull requests
opened here are not merged. To report a problem or propose a change, [contact Mamluk](https://mamluk.net/contact/). Packagist installs every package from
these mirrors, and each one is released under the MIT licence.

| | |
|---|---|
| **Start here** | [starter](https://github.com/kipchak-dev/starter) · [examples](https://github.com/kipchak-dev/examples) · [core](https://github.com/kipchak-dev/core) · [identity](https://github.com/kipchak-dev/identity) |
| **Foundation** | [config](https://github.com/kipchak-dev/driver-config) · [logger](https://github.com/kipchak-dev/driver-logger) · [http](https://github.com/kipchak-dev/driver-http) · [error](https://github.com/kipchak-dev/middleware-error) |
| **Data and storage** | [doctrine](https://github.com/kipchak-dev/driver-doctrine) · [couchdb](https://github.com/kipchak-dev/driver-couchdb) · [clickhouse](https://github.com/kipchak-dev/driver-clickhouse) · [vector](https://github.com/kipchak-dev/driver-vector) · [s3](https://github.com/kipchak-dev/driver-s3) · [sftp](https://github.com/kipchak-dev/driver-sftp) · [git](https://github.com/kipchak-dev/driver-git) |
| **Caching** | [filecache](https://github.com/kipchak-dev/driver-filecache) · [memcached](https://github.com/kipchak-dev/driver-memcached) · [response-cache](https://github.com/kipchak-dev/middleware-response-cache) |
| **Messaging** | [nats](https://github.com/kipchak-dev/driver-nats) · [rabbitmq](https://github.com/kipchak-dev/driver-rabbitmq) |
| **AI** | [anthropic](https://github.com/kipchak-dev/driver-anthropic) · [openai](https://github.com/kipchak-dev/driver-openai) |
| **Security** | [auth-key](https://github.com/kipchak-dev/middleware-auth-key) · [auth-jwks](https://github.com/kipchak-dev/middleware-auth-jwks) · [auth-hmac](https://github.com/kipchak-dev/middleware-auth-hmac) · [subashi](https://github.com/kipchak-dev/middleware-subashi) (WAF) · [clamav](https://github.com/kipchak-dev/driver-clamav) |
| **Operations** | [feature-flags driver](https://github.com/kipchak-dev/driver-feature-flags) · [feature-flags middleware](https://github.com/kipchak-dev/middleware-feature-flags) · [cloudflare-dns](https://github.com/kipchak-dev/driver-cloudflare-dns) · [cloudns](https://github.com/kipchak-dev/driver-cloudns) |

Each package's installation, configuration and use are documented on [kipchak.dev](https://kipchak.dev/ecosystem).
Coding assistants can read the documentation index at [kipchak.dev/llms.txt](https://kipchak.dev/llms.txt), and the
starter includes an `AGENTS.md` file.

## Kipchak Enterprise

[Kipchak Enterprise](https://kipchak.dev/enterprise) adds 18 drivers and middleware for clustering, search, streaming,
observability, policy and advanced authentication, with ticketed support and a published roadmap. Enterprise packages
are distributed privately to customers and are not published on GitHub.

## From Mamluk

Kipchak is developed by [Mamluk](https://mamluk.net), which also builds:

| | |
|---|---|
| <a href="https://bke.bahriya.cloud"><img src="./logos/bke.svg" alt="" width="48" /></a> | [**Bahriya Kubernetes Engine**](https://bke.bahriya.cloud)<br />An enterprise Kubernetes distribution developed and supported from within the GCC. |
| <a href="https://tersane.bahriya.cloud"><img src="./logos/tersane.svg" alt="" width="48" /></a> | [**Bahriya Tersane**](https://tersane.bahriya.cloud)<br />Production Helm charts for the platform above a Kubernetes cluster, licensed for on-premise use. |
| <a href="https://bahriya.cloud"><img src="./logos/bahriya.svg" alt="" width="48" /></a> | [**Bahriya**](https://bahriya.cloud)<br />A public container cloud, powered by the Bahriya Kubernetes Engine. |

---

<div align="center">

<a href="https://mamluk.net"><img src="./logos/mamluk.svg" alt="Mamluk" width="56" /></a>

[mamluk.net](https://mamluk.net) · [Products](https://mamluk.net/products/) · [Journal](https://mamluk.net/journal/) · [Contact](https://mamluk.net/contact/)

</div>
