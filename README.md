<p align="center">
  <img src="arconia-logo.png" alt="Arconia" width="200" />
</p>

<h1 align="center">Arconia Templates</h1>

<p align="center">
  A catalog of templates to bootstrap <a href="https://spring.io/projects/spring-boot">Spring Boot</a> projects using the <a href="https://docs.arconia.io/arconia-cli">Arconia CLI</a>.
</p>

<p align="center">
  <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="Apache 2.0 License" /></a>
</p>

---

## 📦&nbsp; Templates

| Name | Description |
|------|-------------|
| `server-http` | Application using Spring Web MVC, Actuator, and OpenTelemetry. |
| `server-http-jdbc` | Application using Spring Web MVC, Spring Data JDBC, Flyway, PostgreSQL, and OpenTelemetry. |
| `server-ai-rag` | Application using Spring AI, Ollama, PGvector, Docling, JobRunr, and OpenTelemetry. |

## ⚡&nbsp; Quick Start

**1. Add the Arconia Templates catalog**

Register the catalog with the Arconia CLI so its templates are available locally:

```shell
arconia template catalog add \
  --name arconia-templates \
  --ref ghcr.io/arconia-io/arconia-templates/catalog
```

**2. Browse available templates**

List all templates from your registered catalogs:

```shell
arconia template ls
```

**3. Create a project from a template**

Use a template name (resolved automatically from the catalog):

```shell
arconia create --name my-app --template server-ai-rag
```

Or use the full OCI reference directly:

```shell
arconia create --name my-app --template ghcr.io/arconia-io/arconia-templates/server-ai-rag
```

## 📙&nbsp; Documentation

The [Arconia CLI documentation](https://docs.arconia.io/arconia-cli) covers all available commands, options, and workflows in detail.

## 🖊️&nbsp; License

This project is licensed under the **Apache License 2.0**. See [LICENSE](LICENSE) for more information.
