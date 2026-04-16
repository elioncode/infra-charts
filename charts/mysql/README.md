# mysql

Lightweight MySQL 5.7 chart intended for shared or PR environments.

## Goals

- Keep the chart small and predictable
- Default to MySQL 5.7.44
- Support `existingSecret` for passwords
- Use only ephemeral storage (`emptyDir`) for temporary environments
- Be usable as a standalone chart or as a subchart inside business realms

## Main values

- `enabled`: whether the chart is enabled when used as a dependency
- `fullnameOverride`: stable service name, defaults to `mysql`
- `auth.existingSecret`: existing secret name for passwords
- `auth.database`: optional database to auto-create on first boot
