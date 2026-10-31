# ZoneMobStack 1.0.1

## English

Server-only tier-aware hostile mob stacking. Clients do not install it. Same type and matching ZoneLevelUp tier are required; unranked mobs only merge with unranked mobs. ZoneLevelUp is optional. Configure radio_bloques, maximo_por_pila and mobs_excluidos in world/serverconfig/zonemobstack-server.toml. Version1.0.1 bounds candidate processing, avoids duplicate death scheduling and preserves stack names. Bosses and special encounters are excluded.

## Español

Apilado solo de servidor por tipo y rango; los clientes no instalan este JAR. Mismo tipo y rango de ZoneLevelUp, o ambos sin rango. ZoneLevelUp es opcional. Configura radio_bloques, maximo_por_pila y mobs_excluidos en world/serverconfig/zonemobstack-server.toml. 1.0.1 limita candidatos, evita muertes programadas duplicadas y conserva nombres. Se excluyen jefes y encuentros especiales.


| Side / Lado | Version | File |
|---|---|---|
| server | 1.0.1 | `zonemobstack-1.0.1-protected.jar` |

## Dependencies / Dependencias

- **server**: zonelevelup: Optional Dependency ([0,))

## Installation / Instalación

Install only the file for each side. Never mix two versions or both side distributions in one mods folder. Back up the world and preserve TOML/player data. Dedicated-server-only mods do not belong in a client modpack.

Instala solo el archivo del lado correspondiente. No mezcles versiones ni ambos JAR en una carpeta mods. Respalda mundo y conserva TOML/progreso. Los mods exclusivos de servidor no van en el modpack de cliente.

Protected public files retain features without distributing private source, mappings or production configuration/account data. File/resources/shared schemas and isolated server startup/clean save were checked; no new GUI/full-modpack or live multiplayer test was performed. File availability depends on CurseForge approval.

Los archivos públicos conservan funciones con protección, sin fuentes, mappings ni datos privados. Se verificaron archivos/esquemas y arranque/cierre local aislado; no una nueva prueba gráfica o multijugador real. Disponibilidad sujeta a aprobación de CurseForge.

## Ownership / Titularidad

Original ZONE code and artwork © Elgochogms. All Rights Reserved. Public documentation repository only; source and mappings remain private.
