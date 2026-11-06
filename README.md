# ZoneMobStack

Server-side grouping of compatible hostile mobs into visible xN stacks while preserving individual members and normal death events.

Agrupación de mobs hostiles compatibles en pilas visibles xN, conservando miembros individuales y eventos normales de muerte.

## Current release / Entrega actual — 2026-11-06

Minecraft **1.20.1**, Forge **47.x** (47.4.x for this release set), Java **17**. File availability follows CurseForge approval. / Disponibilidad de archivos según aprobación de CurseForge.

| Side / Lado | Version / Versión |
|---|---|
| Server only / Solo servidor | 1.0.2 |

**Compatibility / Compatibilidad:** No client network requirement / Sin requisito de canal cliente.

[Downloads / Descargas](https://www.curseforge.com/projects/1775776/files) · [Release guide / Guía de novedades](RELEASE-2026-11-06.md) · [Configuration / Configuración](CONFIGURATION.md)

## English — Requirements and quick start

Forge 47.4.x/Java 17; server only. ZoneLevelUp is optional for difficulty-tier integration. No Core dependency and no MobStack client JAR required.

Install only on the dedicated server. Nearby hostiles of the same type and tier can merge; each confirmed death consumes one member and restores the next. Keep the world recovery data when updating.

### What changed

- Persistent recovery queue survives rejected spawns and normal restarts, waiting for entity chunks without force-loading them.
- Cancelled deaths do not consume members; duplicate death events share one recovery. Names remain correct across merges, tier labels and slime splitting.
- Excludes expedition markers/minions and active vanilla raids; bounded arrival, recovery and label processing avoids repeated full-world scans.

## Español — Requisitos e inicio

Forge 47.4.x/Java 17; solo servidor. ZoneLevelUp opcional para rangos de dificultad. Sin dependencia de Core ni JAR MobStack requerido en cliente.

Instala solo en el servidor dedicado. Hostiles cercanos del mismo tipo y rango pueden unirse; cada muerte confirmada consume uno y restaura el siguiente. Conserva datos de recuperación al actualizar.

### Novedades

- Cola persistente ante reapariciones rechazadas y reinicios normales; espera chunks de entidades sin forzar carga.
- Muertes canceladas no consumen miembros y eventos duplicados comparten recuperación. Nombres correctos en fusiones, rangos y división de slimes.
- Excluye expediciones/esbirros e incursiones vanilla activas; procesa llegadas, recuperaciones y etiquetas con límites sin recorrer continuamente todo el mundo.

## Updating / Actualizar

Stop the affected instance, back up world/configuration, replace only the previous same-mod/same-side JAR and retain player data. Never install the dedicated and client JARs of one mod together. / Detén la instancia correspondiente, respalda mundo/configuración y sustituye solo el JAR del mismo mod y lado conservando datos. Nunca instales juntos los JAR dedicado y cliente del mismo mod.

## Validation scope / Alcance de verificación

An isolated Forge 47.4.10 server tested cancelled deaths, repeated spawn rejection, restart recovery, merge/count limits and integration with LevelUp r55. Real-player loot/XP, client connection without the JAR, full modpack and loaded TPS remain untested; forced-crash durability is not guaranteed.

Forge 47.4.10 aislado probó muertes canceladas, rechazos, reinicio, fusiones/límites e integración LevelUp r55. Faltan XP/botín con jugador real, conexión sin JAR cliente, modpack y TPS bajo carga; sin garantía ante cierres forzados.

## Rights / Derechos

Original ZONE code and assets © Elgochogms; existing licenses and third-party notices remain applicable. This repository provides public documentation. / Código y recursos originales ZONE © Elgochogms; se conservan licencias y avisos de terceros. Este repositorio contiene documentación pública.
