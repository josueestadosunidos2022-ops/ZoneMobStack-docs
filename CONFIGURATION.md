# ZoneMobStack — Configuration / Configuración (2026-11-06)

| Side / Lado | Version / Versión |
|---|---|
| Server only / Solo servidor | 1.0.2 |

## Server configuration / Configuración del servidor

File: `<mundo>/serverconfig/zonemobstack-server.toml`. Edit with the server stopped for controlled changes. / Edita con servidor detenido para cambios controlados.

| Key / Clave | Default / Inicial | Range or meaning / Rango o uso |
|---|---|---|
| `radio_bloques` | 6 | Search on each axis,1–16 / Búsqueda por eje |
| `maximo_por_pila` | 16 | Original mobs per stack,2–64 / Originales por pila |
| `mobs_excluidos` | Wither and dragon / Wither y dragón | Additional excluded entity IDs / IDs excluidos adicionales |

Known/tagged bosses, ZoneLevelUp/ZoneDungeons special mobs, babies, passengers, mounts, leashed mobs and genuine user-named mobs are excluded. Manual names block new merges. / Se excluyen jefes, especiales, bebés, pasajeros, monturas, atados y nombres propios del usuario; estos últimos bloquean fusiones nuevas.

Individual snapshots over 65536 SNBT characters and queues over 262144 are rejected. Processing caps:128 arrival candidates and16 recovery checks per dimension per tick;32 labels every 5 ticks. Failed recovery retries approximately every 100 ticks within its budget. / Límites SNBT y trabajo indicados; recuperación fallida se reintenta aproximadamente cada100 ticks.

## Data and rewards / Datos y recompensas

Preserve each dimension's `data/zonemobstack_revivals.dat`; it may contain pending mobs. Recovery waits until entity chunks load and does not keep them force-loaded. Existing stack/configuration formats are retained. / Conserva el archivo de pendientes por dimensión; espera chunks sin forzarlos y conserva formatos anteriores.

Each member retains its own data. A confirmed death normally restores the next member next tick. Loot/XP use normal death events rather than multiplication by stack size. Changing LevelUp tier configuration can deliberately reclassify mobs; MobStack does not override that choice. / Cada miembro conserva datos; muerte confirmada restaura siguiente normalmente al próximo tick. Botín/XP usan eventos normales, sin multiplicación artificial. Cambiar rangos LevelUp puede reclasificar mobs.

[Current release / Entrega actual](RELEASE-2026-11-06.md) · [README](README.md).
