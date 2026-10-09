# 🔌 Especificación Técnica y API — ProjectJaina_GearScore

[![GitHub](https://img.shields.io/badge/GitHub-DarckRovert%2FProjectJaina_GearScore-black?logo=github)](https://github.com/DarckRovert/ProjectJaina_GearScore)
[![Ecosistema](https://img.shields.io/badge/Ecosistema-WoW%20Per%C3%BA%203.3.5a-gold.svg)](https://wow-peru.lat/)

## 📌 Resumen Arquitectónico
Monorepositorio unificado de GearScore (3.1.16-WP) y BonusScanner (5.3) optimizado para el cálculo exacto de poder de equipo sin bloqueos de caché de ítems.

- **Rol en el Ecosistema:** Suite Comunitaria Monorepo — Puntuación de Equipo
- **Archivo Principal TOC:** `GearScore.toc`
- **Compatibilidad del Motor:** World of Warcraft 3.3.5a (Build 12340)

---

## ⌨️ Comandos de Consola (Slash Commands)
- `/gearscore`: Acceso principal o comando del addon.
- `/gs`: Acceso principal o comando del addon.
- `/bonusscanner`: Acceso principal o comando del addon.
- `/bscan`: Acceso principal o comando del addon.

---

## 📡 Protocolo de Red y Eventos
- `GSY`: Prefijo registrado para sincronización de datos.
- `GSYTRANSMIT`: Prefijo registrado para sincronización de datos.
- `GSY_Request`: Prefijo registrado para sincronización de datos.
- `GSY_Version`: Prefijo registrado para sincronización de datos.

### Eventos del Motor 3.3.5a Gestionados
- `PLAYER_LOGIN` / `ADDON_LOADED`: Inicialización atómica de tablas de configuración y hooks.
- `PLAYER_ENTERING_WORLD`: Sincronización de estado tras transiciones de pantalla o mapa.
- `PLAYER_LOGOUT`: Guardado seguro en disco de las variables locales.

---

## 💾 Persistencia de Datos (SavedVariables)
- `GS_Data`: Almacenamiento estructurado de configuración y estado persistente.
- `GS_Settings`: Almacenamiento estructurado de configuración y estado persistente.
- `BonusScannerConfig`: Almacenamiento estructurado de configuración y estado persistente.

---

## 🛠️ Buenas Prácticas de Integración
1. Toda invocación a funciones públicas debe verificar previamente la existencia del espacio de nombres en `_G`.
2. Las tablas de configuración deben consultarse en modo lectura sin sobreescribir valores por omisión no validados.
3. El intercambio de datos con otros addons debe efectuarse a través del bus oficial `ProjectJaina_Companion` o hooks de eventos estándar.
