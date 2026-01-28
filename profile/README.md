# Reference System Python

The Copernicus Space Component *Reference System* is an open-source software solution allowing to implement, maintain, deploy, operate and monitor Sentinel data processing workflows based on the future re-engineered Level 0, 1, 2 [Sentinel Data processors](https://eopf.copernicus.eu/).

## How to find what you need

This organization has several repositories of different types.
Here, we categorise each repository as follows:

- 🧙 **Documentation repositories** to learn about the project and play with Jupyter notebooks
- 👩‍🍳 **STAC extensions** to extend [STAC](https://stacspec.org) capabilities
- 🐍 **Python repositories** to get client libraries, processing workflows and server applications
- 🧑‍💻 **Infrastructure repositories** to deploy the solution on a Kubernetes cluster

For more information on each repository, see its respective README.

### 🧙 Documentation repositories

| Repository | Status | Description |
| -- | -- | -- |
| [rs-demo](https://github.com/RS-PYTHON/rs-demo) | ![CI](https://github.com/RS-PYTHON/rs-demo/actions/workflows/run_demos.yml/badge.svg?branch=develop) | Collection of [Jupyter](https://jupyter.org/) notebooks showcasing the latest features of the system |
| [rs-documentation](https://github.com/RS-PYTHON/rs-documentation) | ![CI](https://github.com/RS-PYTHON/rs-documentation/actions/workflows/generate-documentation.yml/badge.svg?branch=develop) | This repository gathers and generates the [online documentation](https://home.rs-python.eu/rs-documentation/) |
| [RS-PYTHON.github.io](https://github.com/RS-PYTHON/RS-PYTHON.github.io) |  | This repository contains the template and data to generate rs-python [landing page](https://home.rs-python.eu/) website |

### 👩‍🍳 STAC extensions

| Repository | Status | Description |
| -- | -- | -- |
| [auxip-stac-extension](https://github.com/RS-PYTHON/auxip-stac-extension) | ![CI](https://github.com/RS-PYTHON/auxip-stac-extension/actions/workflows/test.yaml/badge.svg?branch=main) | Allows to describe Copernicus [Auxiliary Data](https://sentiwiki.copernicus.eu/web/copernicus-operations#CopernicusOperations-AuxiliaryDataGathering) files as STAC items |
| [cadip-stac-extension](https://github.com/RS-PYTHON/cadip-stac-extension) | ![CI](https://github.com/RS-PYTHON/cadip-stac-extension/actions/workflows/test.yaml/badge.svg?branch=main) | Allows to describe Copernicus [CADIP sessions](https://sentiwiki.copernicus.eu/web/copernicus-operations#CopernicusOperations-X-BandAcquisition) from Acquisition Ground Stations as STAC items |
| [ownership-stac-extension](https://github.com/RS-PYTHON/ownership-stac-extension) | ![CI](https://github.com/RS-PYTHON/ownership-stac-extension/actions/workflows/test.yaml/badge.svg?branch=main) | Allows to express ownership of STAC collections and items |
| [download-stac-api-extension](https://github.com/RS-PYTHON/download-stac-api-extension) | ![CI](https://github.com/RS-PYTHON/download-stac-api-extension/actions/workflows/main.yml/badge.svg?branch=main) | STAC API Extension that adds a dedicated endpoint to download an asset |

### 🐍 Python repositories

| Repository | Status | Description |
| -- | -- | -- |
| [rs-server](https://github.com/RS-PYTHON/rs-server) | ![CI](https://github.com/RS-PYTHON/rs-server/actions/workflows/publish-binaries.yml/badge.svg?branch=develop) | The rs-server components provide [STAC](https://stacspec.org) services for catalog and external data access (from CADIP, AUXIP, LTA and PRIP), with fine access control |
| [rs-client-libraries](https://github.com/RS-PYTHON/rs-client-libraries) | ![CI](https://github.com/RS-PYTHON/rs-client-libraries/actions/workflows/publish-binaries.yml/badge.svg?branch=develop) | Collection of Python modules: rs-client library (which simplifies calling rs-server services) and processing workflows |
| [rs-dpr-service](https://github.com/RS-PYTHON/rs-dpr-service) | ![CI](https://github.com/RS-PYTHON/rs-dpr-service/actions/workflows/publish-binaries.yml/badge.svg?branch=develop) | Service that allows to retrieve [tasktables](https://cpm.pages.eopf.copernicus.eu/eopf-cpm/main/processor-orchestration-guide/tasktables.html) and [trigger DPR/EOPF processors](https://cpm.pages.eopf.copernicus.eu/eopf-cpm/main/processor-orchestration-guide/triggering-usage.html) in a Dask cluster |
| [pygeofilter](https://github.com/RS-PYTHON/pygeofilter) | ![CI](https://github.com/RS-PYTHON/pygeofilter/actions/workflows/main.yml/badge.svg?branch=rspy) | Fork of pygeofilter to get [CQL2](https://docs.ogc.org/is/21-065r2/21-065r2.html) fixes without waiting for a new upstream release |
| [operational-services](https://github.com/RS-PYTHON/operational-services) | ![CI](https://github.com/RS-PYTHON/operational-services/actions/workflows/publish-binaries.yml/badge.svg?branch=develop) | Operational services required for Reference System |
| [testmeans](https://github.com/RS-PYTHON/rs-testmeans) | ![CI](https://github.com/RS-PYTHON/rs-testmeans/actions/workflows/publish-docker.yml/badge.svg?branch=develop) | Test means and mockups to valide Reference System CSC interfaces |

### 🧑‍💻 Infrastructure repositories

| Repository | Status | Description |
| -- | -- | -- |
| [rs-helm](https://github.com/RS-PYTHON/rs-helm) | ![CI](https://github.com/RS-PYTHON/rs-helm/actions/workflows/lint-test.yaml/badge.svg?branch=develop) | This repository provides [Helm charts](https://helm.sh/) for deploying rs-server services |
| [rs-infra-core](https://github.com/RS-PYTHON/rs-infra-core) | ![CI](https://github.com/RS-PYTHON/rs-infra-core/actions/workflows/test-deployment.yml/badge.svg?branch=develop) | This repository provides the [Ansible playbooks](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_intro.html) to deploy the basic Kubernetes infrastructure components |
| [rs-infra-monitoring](https://github.com/RS-PYTHON/rs-infra-monitoring) | ![CI](https://github.com/RS-PYTHON/rs-infra-monitoring/actions/workflows/test-deployment.yml/badge.svg?branch=develop) | A set of monitoring components to deploy on top of core infrastructure |
| [rs-server-deployment](https://github.com/RS-PYTHON/rs-server-deployment) | ![CI](https://github.com/RS-PYTHON/rs-server-deployment/actions/workflows/test-deployment.yml/badge.svg?branch=develop) | A set of components to deploy rs-server services on top of core infrastructure |
| [rs-workflow-env](https://github.com/RS-PYTHON/rs-workflow-env) | ![CI](https://github.com/RS-PYTHON/rs-workflow-env/actions/workflows/test-deployment.yml/badge.svg?branch=develop) | A set of components to support processing orchestration on top of core infrastructure |
| [rs-workflow-deployment](https://github.com/RS-PYTHON/rs-workflow-deployment) | ![CI](https://github.com/RS-PYTHON/rs-workflow-deployment/actions/workflows/test-deployment.yml/badge.svg?branch=develop) | A set of components to deploy rs-client prefect-flow from ansible on top of core infrastructure |

## Licensing


The code in this project is licensed under Apache License 2.0.

---

![](banner_logo.jpg)

This project is funded by the EU and ESA.
