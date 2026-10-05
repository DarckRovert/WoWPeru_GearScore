# 🌐 Registro de Ecosistema — WoWPeru_GearScore

Ficha técnica oficial de registro en la infraestructura multi-addon de **WoW Perú - Reino Andino**.

---

## 1. Identidad de la Suite

| Campo | Valor |
|---|---|
| **Nombre Técnico** | `GearScore Suite` |
| **Título en Cliente** | `GearScore` & `BonusScanner Continued 5.3` |
| **Versión** | `3.1.16-WP` |
| **Tipo de Sistema** | Evaluación Cuantitativa de Equipamiento e Inspección |
| **Repositorio GitHub** | [DarckRovert/WoWPeru_GearScore](https://github.com/DarckRovert/WoWPeru_GearScore) |
| **Directorios de Instalación** | `Interface\AddOns\GearScore\` y `Interface\AddOns\BonusScanner\` |

---

## 2. Persistencia de Datos

| Variable Global | Tipo | Ámbito | Propósito |
|---|---|---|---|
| `GS_Data` | Tabla Lua (`SavedVariables`) | Por Cuenta | Base de datos de inspecciones previas y promedios |
| `GS_Settings` | Tabla Lua (`SavedVariables`) | Por Cuenta | Opciones de visualización, escala y tooltips |
| `BonusScannerConfig` | Tabla Lua (`SavedVariables`) | Por Cuenta | Opciones de escaneo de bonificaciones |

---

## 3. Matriz de Integración

| Sistema Coexistente | Modo de Interacción | Flujo de Datos |
|---|---|---|
| **`WoWPeru_Companion`** | Detección / Telemetría | Verifica presencia y lectura de GS para balance |
| **`WoWPeru_DragonflightUI`** | Inyección en Tooltip | Se renderiza sin interferir con estilos modernos |
