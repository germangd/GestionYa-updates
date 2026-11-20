# GestionYa-updates

Repo auxiliar para alojar instaladores / releases de descarga.

## Circuito real de updates (GestiónYa Ventas 2.0)

La app Electron usa `electron-updater` contra el feed de **license-api**:

- `GET /v1/app-updates/latest.yml`
- `GET /v1/app-updates/win7.yml` (ia32 / Win7)

Fuente canónica: https://github.com/germangd/license-api (`src/routes/appUpdates.js`).

Este repositorio puede seguir usándose para hostear los binarios (URLs en `download_url` del feed), pero **no** es el servidor del feed YAML.
