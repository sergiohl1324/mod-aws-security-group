# Changelog — mod-aws-security-group

Todos los cambios notables de este módulo están documentados en este archivo.
Formato basado en [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
Versionamiento semántico según [SemVer](https://semver.org/).

---

## [v0.1.0] — 2026-06-19

### Added
- Primer tag formal de versión (el módulo ya existía como wrapper de `terraform-aws-modules/security-group`, vendoreado en 2023, pero nunca se había versionado con SemVer/tags de git).
- `versions.tf`: pin de `required_version` y del provider `hashicorp/aws ~> 5.0` (antes solo tenía `required_version = ">= 0.13"`, sin pin de provider).
- `locals.tf`: bloque `common_tags` (Project, Environment, ManagedBy) mergeado con `var.tags`, reemplazando el placeholder `additional_local_variable`.
- `variables.tf`: nuevas variables `project` y `environment` para tagging.
- `config/terraform-docs.yml` para generación de README.

### Notes
- `rules.tf`, `update_groups.sh` y `modules/` no se modificaron — fuera de alcance.
