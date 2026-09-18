# jenkins-job-one

Pipeline job that deploys **payments-api** to **dev**.

- [`Jenkinsfile`](Jenkinsfile) — reads `config.json` and passes its values into `runConfigJob(serviceName: ..., environment: ...)`.
- [`config.json`](config.json) — parameters consumed by the shared step:
  ```json
  { "serviceName": "payments-api", "environment": "dev" }
  ```
- [`config.xml`](config.xml) — importable Jenkins pipeline-job definition.

The logic lives entirely in the shared library
(`grvsoni/jenkins-shared-library`); this repo only supplies the config values.
# jenkins-job-one
