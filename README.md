# gcloud-terraform

## A repository that adds the `gcloud`, `terraform` and `firebase` command line tools to a project for CI/CD or for running emulators

### Requirements

1. [Docker](https://docker.com)
1. A GCP / Firebase project

### Setup

- Add your auth credentials inside the respective files in `.docker/.env/`.
- Set the path of your project in the `docker-compose.yml` file.
- Optionally run `. ./.docker/alias` to add aliases to your current shell.

### Examples

- Run terraform by running `docker-compose run --rm terraform <cmd>`
- Run a gcloud emulator by running the alias `emulator <cmd>` e.g. `emulator pubsub start`
- Run a firebase emulator by running the alias `firebase-tools emulators:<cmd>` e.g. `firebase-tools emulators:start`
