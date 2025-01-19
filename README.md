[![tests](https://github.com/ddev/ddev-addon-template/actions/workflows/tests.yml/badge.svg)](https://github.com/ddev/ddev-addon-template/actions/workflows/tests.yml) ![project is maintained](https://img.shields.io/maintenance/yes/2024.svg)

# ddev-ollama <!-- omit in toc -->


## What is ddev-ollama?

ddev-ollama adds local instance of [Ollama](https://ollama.com/) to a ddev project.

The code is largely based on the work done in https://github.com/valiantlynx/ollama-docker

## Getting started

1. Install the plugin with `ddev get valthebald/ddev-ollama`
2. Restart DDEV to install it with `ddev restart`#
3. Access http://localhost:8080 in your browser (TBD port configurable)

## Using with Drupal AI module

1. Install and enable [Ollama provider module](https://www.drupal.org/project/ai_provider_ollama)
2. In provider settings `/admin/config/ai/providers/ollama` set the Host to `http://host.docker.internal` and port to `7869` (TBD make this configurable)