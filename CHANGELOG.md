# Changelog — mod-aws-security-group

All notable changes to this module are documented in this file.
Format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
Versioning follows [SemVer](https://semver.org/).

---

## [v0.1.0] — 2026-06-19

### Added
- First formal version tag (the module already existed as a wrapper of `terraform-aws-modules/security-group`, vendored in 2023, but had never been versioned with SemVer/git tags).
- `versions.tf`: pinning `required_version` and the `hashicorp/aws ~> 5.0` provider (previously only had `required_version = ">= 0.13"`, with no provider pin).
- `locals.tf`: `common_tags` block (Project, Environment, ManagedBy) merged with `var.tags`, replacing the `additional_local_variable` placeholder.
- `variables.tf`: new `project` and `environment` variables for tagging.
- `config/terraform-docs.yml` for README generation.

### Notes
- `rules.tf`, `update_groups.sh` and `modules/` were not modified — out of scope.
