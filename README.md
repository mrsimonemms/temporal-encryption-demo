# temporal-encryption-demo

A Temporal workflow to demonstrate encryption

<!-- toc -->

* [Quick Start](#quick-start)
* [Purporse](#purporse)
* [Contributing](#contributing)
  * [Open in a container](#open-in-a-container)
  * [Commit style](#commit-style)

<!-- Regenerate with "pre-commit run -a markdown-toc" -->

<!-- tocstop -->

## Quick Start

> This will run in [Temporal Cloud](https://cloud.temporal.io). If you wish to use
> mTLS instead, use `TEMPORAL_TLS_CLIENT_CERT_PATH` and `TEMPORAL_TLS_CLIENT_KEY_PATH`
> environment variables instead.

```sh
docker run -it --rm \
  -e TEMPORAL_API_KEY=${TEMPORAL_API_KEY} \
  -e TEMPORAL_ADDRESS=${TEMPORAL_ADDRESS} \
  -e TEMPORAL_NAMESPACE=${TEMPORAL_NAMESPACE} \
  -e TEMPORAL_TLS=${TEMPORAL_TLS} \
  ghcr.io/mrsimonemms/temporal-encryption-demo
```

## Purporse

This is a demo of encryption, designed to run as a schedule. As a Solutions Architect,
a lot of my job is demonstrating the power of Temporal to new users. When demonstrating
the Cloud, I want to show how to encrypt and decrypt data within the UI. Very often,
I can't actually find an example of encrypted data.

So this runs on a schedule so I've always got something to show.

This uses [Zigflow](https://zigflow.dev) as a Temporal DSL for ease of development.

## Contributing

### Open in a container

* [Open in a container](https://code.visualstudio.com/docs/devcontainers/containers)

### Commit style

All commits must be done in the [Conventional Commit](https://www.conventionalcommits.org)
format.

```git
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```
