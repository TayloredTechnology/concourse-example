# Concourse Example

Sample repo to show tracking or wrapped deployment functionality for a single application with no dependencies.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Taylored Technology's [**Concourse**](https://concourse.tayloredtechnology.net) needs to be deployed into your container orchestration framework

## Deployment

Example Applications can be deployed in one of several ways:
- via **Concourse**'s [tracking functionality](https://concourse.tayloredtechnology.net/api/tracker)
- via baking this repo's *concourse.yaml* file into your **Concourse** container image in the */concourse/default* directory as *{{name}}.app.yaml* where {{name}} is custom defined
- via dynamically pushing this and other desired *app.yaml* files into the running **Concourse** master image's */deploy* directory... if this option is chosen, ensure that *namespaces.yaml* is also pushed into this directory

## License

This project is licensed under the Mozilla Public License Version 2.0 - see the [LICENSE](LICENSE) file for details

## Acknowledgments

- CoreOS's Tectonic for the sample app
