# 🇵🇪 Project Jaina — GearScore Suite (v3.1.16-WP + BonusScanner 5.3)

**Versión:** 3.1.16-WP  
**Autores Originales:** Mirrikat45 (GearScore) & Tristanian (BonusScanner)  
**Mantenimiento & Empaquetado:** DarckRovert & Project Jaina Staff  
**Servidor Destino:** [Project Jaina](https://wow-peru.lat/) — Reino Andino  
**Entorno de Ejecución:** World of Warcraft 3.3.5a (Build 12340) | Lua 5.1  
**Repositorio Oficial:** [DarckRovert/ProjectJaina_GearScore](https://github.com/DarckRovert/ProjectJaina_GearScore)  

---

[![WoW Client](https://img.shields.io/badge/WoW%20Client-3.3.5a%20(Build%2012340)-blue.svg)](https://wow-peru.lat/)
[![Servidor](https://img.shields.io/badge/Servidor-WoW%20Perú-gold.svg)](https://wow-peru.lat/)
[![Version](https://img.shields.io/badge/version-3.1.16--WP-brightgreen.svg)](https://github.com/DarckRovert/ProjectJaina_GearScore/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 🌟 Descripción General

**ProjectJaina_GearScore** es la suite unificada de inspección de equipo para WoW 3.3.5a, integrando en un solo repositorio **GearScore** y su motor de análisis de bonificaciones **BonusScanner**.

Permite evaluar con precisión el nivel de equipamiento de tu personaje y de jugadores inspeccionados, asignando puntuaciones ponderadas según ranura de objeto, nivel de objeto (iLvl), calidad y estadísticas.

```
┌────────────────────────────────────────────────────────────────────────┐
│                   SUITE GEARSCORE + BONUSSCANNER                       │
├────────────────────────┬──────────────────────┬────────────────────────┤
│ ⚖️ CÁLCULO PONDERADO   │ 🔍 INSPECCIÓN RÁPIDA │ 🧩 ZERO-DEPENDENCY LOSS│
│ Puntuación matemática  │ Tooltips enriquecidos│ BonusScanner integrado │
│ por ranura y calidad   │ en hover e inspect   │ para prevenir errores  │
└────────────────────────┴──────────────────────┴────────────────────────┘
```

---

## 📦 Componentes Incluidos

1. **`GearScore` (v3.1.16):**
   - Interfaz principal, visualización en marco de personaje, cálculo de medias y soporte LDB (LibDataBroker).
   - Comandos principales: `/gs`, `/gearscore`.
2. **`BonusScanner` (v5.3):**
   - Escáner acumulativo de estadísticas de equipo, gemas y encantamientos que alimenta las fórmulas de cálculo de GearScore.

---

## 📥 Instalación en el Cliente WoW

1. Descarga el repositorio o release comprimido en `.zip`.
2. Extrae las 2 carpetas (`GearScore` y `BonusScanner`) directamente dentro de:
   ```
   World of Warcraft/Interface/AddOns/
   ```
3. Inicia el juego y comprueba que ambos accesorios aparezcan marcados en la lista de AddOns.
