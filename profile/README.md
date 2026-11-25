# Reference System Python

The Copernicus Space Component *Reference System* is an open-source software solution allowing to implement, maintain, deploy, operate and monitor Sentinel data processing workflows based on the future re-engineered Level 0, 1, 2 [Sentinel Data processors](https://eopf.copernicus.eu/).

## How to find what you need

This organization has several repositories of different types.
Here, we categorise each repository as follows:

- 🧙 **Documentation repositories** to learn about the project and play with Jupyter notebooks
- 👩‍🍳 **STAC extensions** to extend [STAC](https://stacspec.org) capabilities
- 🐍 **Python repositories** to get client libraries, processing workflows and server applications
- 🧑‍💻 **Infrastructure repositories** to deploy the solution on a Kubernetes cluster
- 🛠 **Tool repositories** to share the CI/CD workflows and actions of all the repositories

For more information on each repository, see its respective README. The *Open PRs* column shows the number of open pull requests of each repository (e.g. the Dependabot updates to review).

<table>
  <tr>
    <th>Repository</th>
    <th>Status</th>
    <th>Open PRs</th>
    <th>Description</th>
  </tr>
  <tr>
    <th colspan="4" align="left">🧙 Documentation repositories</th>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-demo">rs-demo</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-demo/actions/workflows/run_demos.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-demo/actions/workflows/run_demos.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-demo/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-demo?label=PRs" alt="PRs"></a></td>
    <td>Collection of <a href="https://jupyter.org/">Jupyter</a> notebooks showcasing the latest features of the system</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-documentation">rs-documentation</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-documentation/actions/workflows/generate-documentation.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-documentation/actions/workflows/generate-documentation.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-documentation/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-documentation?label=PRs" alt="PRs"></a></td>
    <td>This repository gathers and generates the <a href="https://home.rs-python.eu/rs-documentation/">online documentation</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/RS-PYTHON.github.io">RS-PYTHON.github.io</a></td>
    <td></td>
    <td><a href="https://github.com/RS-PYTHON/RS-PYTHON.github.io/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/RS-PYTHON.github.io?label=PRs" alt="PRs"></a></td>
    <td>This repository contains the template and data to generate rs-python <a href="https://home.rs-python.eu/">landing page</a> website</td>
  </tr>
  <tr>
    <th colspan="4" align="left">👩‍🍳 STAC extensions</th>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/cadip-stac-extension">cadip-stac-extension</a></td>
    <td><a href="https://github.com/RS-PYTHON/cadip-stac-extension/actions/workflows/test.yaml?query=branch%3Amain"><img src="https://github.com/RS-PYTHON/cadip-stac-extension/actions/workflows/test.yaml/badge.svg?branch=main" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/cadip-stac-extension/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/cadip-stac-extension?label=PRs" alt="PRs"></a></td>
    <td>Allows to describe Copernicus <a href="https://sentiwiki.copernicus.eu/web/copernicus-operations#CopernicusOperations-X-BandAcquisition">CADIP sessions</a> from Acquisition Ground Stations as STAC items</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/ownership-stac-extension">ownership-stac-extension</a></td>
    <td><a href="https://github.com/RS-PYTHON/ownership-stac-extension/actions/workflows/test.yaml?query=branch%3Amain"><img src="https://github.com/RS-PYTHON/ownership-stac-extension/actions/workflows/test.yaml/badge.svg?branch=main" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/ownership-stac-extension/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/ownership-stac-extension?label=PRs" alt="PRs"></a></td>
    <td>Allows to express ownership of STAC collections and items</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/download-stac-api-extension">download-stac-api-extension</a></td>
    <td><a href="https://github.com/RS-PYTHON/download-stac-api-extension/actions/workflows/main.yml?query=branch%3Amain"><img src="https://github.com/RS-PYTHON/download-stac-api-extension/actions/workflows/main.yml/badge.svg?branch=main" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/download-stac-api-extension/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/download-stac-api-extension?label=PRs" alt="PRs"></a></td>
    <td>STAC API Extension that adds a dedicated endpoint to download an asset</td>
  </tr>
  <tr>
    <th colspan="4" align="left">🐍 Python repositories</th>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-server">rs-server</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-server/actions/workflows/publish-binaries.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-server/actions/workflows/publish-binaries.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-server/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-server?label=PRs" alt="PRs"></a></td>
    <td>The rs-server components provide <a href="https://stacspec.org">STAC</a> services for catalog and external data access (from CADIP, AUXIP, LTA and PRIP), with fine access control</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-client-libraries">rs-client-libraries</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-client-libraries/actions/workflows/publish-binaries.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-client-libraries/actions/workflows/publish-binaries.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-client-libraries/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-client-libraries?label=PRs" alt="PRs"></a></td>
    <td>Collection of Python modules: rs-client library (which simplifies calling rs-server services) and processing workflows</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-dpr-service">rs-dpr-service</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-dpr-service/actions/workflows/publish-binaries.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-dpr-service/actions/workflows/publish-binaries.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-dpr-service/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-dpr-service?label=PRs" alt="PRs"></a></td>
    <td>Service that allows to retrieve <a href="https://cpm.pages.eopf.copernicus.eu/eopf-cpm/main/processor-orchestration-guide/tasktables.html">tasktables</a> and <a href="https://cpm.pages.eopf.copernicus.eu/eopf-cpm/main/processor-orchestration-guide/triggering-usage.html">trigger DPR/EOPF processors</a> in a Dask cluster</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/opentelemetry-instrumentation-eopf">opentelemetry-instrumentation-eopf</a></td>
    <td><a href="https://github.com/RS-PYTHON/opentelemetry-instrumentation-eopf/actions/workflows/test.yml?query=branch%3Amain"><img src="https://github.com/RS-PYTHON/opentelemetry-instrumentation-eopf/actions/workflows/test.yml/badge.svg?branch=main" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/opentelemetry-instrumentation-eopf/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/opentelemetry-instrumentation-eopf?label=PRs" alt="PRs"></a></td>
    <td>OpenTelemetry instrumentation for EOPF</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-testmeans">rs-testmeans</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-testmeans/actions/workflows/publish-binaries.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-testmeans/actions/workflows/publish-binaries.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-testmeans/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-testmeans?label=PRs" alt="PRs"></a></td>
    <td>Test means and mockups to valide Reference System CSC interfaces</td>
  </tr>
  <tr>
    <th colspan="4" align="left">🧑‍💻 Infrastructure repositories</th>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-helm">rs-helm</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-helm/actions/workflows/lint-test.yaml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-helm/actions/workflows/lint-test.yaml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-helm/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-helm?label=PRs" alt="PRs"></a></td>
    <td>This repository provides <a href="https://helm.sh/">Helm charts</a> for deploying rs-server services</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-infra-core">rs-infra-core</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-infra-core/actions/workflows/test-deployment.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-infra-core/actions/workflows/test-deployment.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-infra-core/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-infra-core?label=PRs" alt="PRs"></a></td>
    <td>This repository provides the <a href="https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_intro.html">Ansible playbooks</a> to deploy the basic Kubernetes infrastructure components</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-infra-monitoring">rs-infra-monitoring</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-infra-monitoring/actions/workflows/test-deployment.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-infra-monitoring/actions/workflows/test-deployment.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-infra-monitoring/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-infra-monitoring?label=PRs" alt="PRs"></a></td>
    <td>A set of monitoring components to deploy on top of core infrastructure</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-server-deployment">rs-server-deployment</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-server-deployment/actions/workflows/test-deployment.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-server-deployment/actions/workflows/test-deployment.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-server-deployment/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-server-deployment?label=PRs" alt="PRs"></a></td>
    <td>A set of components to deploy rs-server services on top of core infrastructure</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-workflow-env">rs-workflow-env</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-workflow-env/actions/workflows/test-deployment.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-workflow-env/actions/workflows/test-deployment.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-workflow-env/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-workflow-env?label=PRs" alt="PRs"></a></td>
    <td>A set of components to support processing orchestration on top of core infrastructure</td>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/rs-workflow-deployment">rs-workflow-deployment</a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-workflow-deployment/actions/workflows/test-deployment.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/rs-workflow-deployment/actions/workflows/test-deployment.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/rs-workflow-deployment/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/rs-workflow-deployment?label=PRs" alt="PRs"></a></td>
    <td>A set of components to deploy rs-client prefect-flow from ansible on top of core infrastructure</td>
  </tr>
  <tr>
    <th colspan="4" align="left">🛠 Tool repositories</th>
  </tr>
  <tr>
    <td><a href="https://github.com/RS-PYTHON/actions">actions</a></td>
    <td><a href="https://github.com/RS-PYTHON/actions/actions/workflows/check-code-quality.yml?query=branch%3Adevelop"><img src="https://github.com/RS-PYTHON/actions/actions/workflows/check-code-quality.yml/badge.svg?branch=develop" alt="CI"></a></td>
    <td><a href="https://github.com/RS-PYTHON/actions/pulls"><img src="https://img.shields.io/github/issues-pr-raw/RS-PYTHON/actions?label=PRs" alt="PRs"></a></td>
    <td>This repository provides reusable GitHub workflows and composite actions for all RS-PYTHON repositories.</td>
  </tr>
</table>

## Licensing


The code in this project is licensed under Apache License 2.0.

---

![](banner_logo.jpg)

This project is funded by the EU and ESA.
