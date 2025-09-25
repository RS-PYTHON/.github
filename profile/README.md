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

| Repository | Description |
| -- | -- |
| [rs-demo](https://github.com/RS-PYTHON/rs-demo) | Collection of [Jupyter](https://jupyter.org/) notebooks showcasing the latest features of the system |
| [rs-documentation](https://github.com/RS-PYTHON/rs-documentation) | This repository gathers and generates the [online documentation](https://home.rs-python.eu/rs-documentation/) |
| [RS-PYTHON.github.io](https://github.com/RS-PYTHON/RS-PYTHON.github.io) | This repository contains the template and data to generate rs-python [landing page](https://home.rs-python.eu/) website |

### 👩‍🍳 STAC extensions

| Repository | Description |
| -- | -- |
| [auxip-stac-extension](https://github.com/RS-PYTHON/auxip-stac-extension) | Allows to describe Copernicus [Auxiliary Data](https://sentiwiki.copernicus.eu/web/copernicus-operations#CopernicusOperations-AuxiliaryDataGathering) files as STAC items |
| [cadip-stac-extension](https://github.com/RS-PYTHON/cadip-stac-extension) | Allows to describe Copernicus [CADIP sessions](https://sentiwiki.copernicus.eu/web/copernicus-operations#CopernicusOperations-X-BandAcquisition) from Acquisition Ground Stations as STAC items |
| [ownership-stac-extension](https://github.com/RS-PYTHON/ownership-stac-extension) | Allows to express ownership of STAC collections and items |
| [download-stac-api-extension](https://github.com/RS-PYTHON/download-stac-api-extension) | STAC API Extension that adds a dedicated endpoint to download an asset |

### 🐍 Python repositories

| Repository | Description |
| -- | -- |
| [rs-server](https://github.com/RS-PYTHON/rs-server) | The rs-server components provide [STAC](https://stacspec.org) services for catalog and external data access (from CADIP, AUXIP, LTA and PRIP), with fine access control |
| [rs-client-libraries](https://github.com/RS-PYTHON/rs-client-libraries) | Collection of Python modules: rs-client library (which simplifies calling rs-server services) and processing workflows |
| [rs-dpr-service](https://github.com/RS-PYTHON/rs-dpr-service) | Service that allows to retrieve [tasktables](https://cpm.pages.eopf.copernicus.eu/eopf-cpm/main/processor-orchestration-guide/tasktables.html) and [trigger DPR/EOPF processors](https://cpm.pages.eopf.copernicus.eu/eopf-cpm/main/processor-orchestration-guide/triggering-usage.html) in a Dask cluster |
| [pygeofilter](https://github.com/RS-PYTHON/pygeofilter) | Fork of pygeofilter to get [CQL2](https://docs.ogc.org/is/21-065r2/21-065r2.html) fixes without waiting for a new upstream release |
| [operational-services](https://github.com/RS-PYTHON/operational-services) | Operational services required for Reference System |

### 🧑‍💻 Infrastructure repositories

| Repository | Description |
| -- | -- |
| [rs-helm](https://github.com/RS-PYTHON/rs-helm) | This repository provides [Helm charts](https://helm.sh/) for deploying rs-server services |
| [rs-infra-core](https://github.com/RS-PYTHON/rs-infra-core) | This repository provides the [Ansible playbooks](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_intro.html) to deploy the basic Kubernetes infrastructure components |
| [rs-infra-monitoring](https://github.com/RS-PYTHON/rs-infra-monitoring) | A set of monitoring components to deploy on top of core infrastructure |
| [rs-server-deployment](https://github.com/RS-PYTHON/rs-server-deployment) | A set of components to deploy rs-server services on top of core infrastructure |
| [rs-workflow-env](https://github.com/RS-PYTHON/rs-workflow-env) | A set of components to support processing orchestration on top of core infrastructure |
| [rs-workflow-env](https://github.com/RS-PYTHON/rs-workflow-deployment) | A set of components to deploy rs-client prefect-flow from ansible on top of core infrastructure |
