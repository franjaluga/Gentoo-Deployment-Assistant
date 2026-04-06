# Gentoo Deployment Assistant (GDA)

**Gentoo Deployment Assistant** es una herramienta diseñada para automatizar las tareas repetitivas de la instalación de Gentoo, manteniendo la transparencia y el control total que los usuarios de esta distribución exigen.

A diferencia de otros instaladores, **GDA** no es una "caja negra". Su objetivo es servir como un asistente de despliegue que permite al usuario revisar cada paso, modificar configuraciones críticas y aprender del proceso.

---

## 🛠 Características Principales

* **Arquitectura Transparente:** Basado en scripts de Bash modulares y legibles.
* **Gestión de Discos:** Automatización del particionamiento y formateo (con soporte para estructuras estándar).
* **Kernel Friendly:** Incluye configuraciones base y scripts para la compilación del kernel.
* **Configuración Optimizada:** Archivos `make.conf` pre-estructurados para facilitar la personalización de `COMMON_FLAGS` y `USE` flags.
* **Enfoque Educativo:** Diseñado para ser ejecutado paso a paso, permitiendo al usuario intervenir en el proceso de `chroot`.

## 🚀 Filosofía: "The Gentoo Way"

Este proyecto reconoce que la instalación manual es el mejor método para aprender Gentoo. GDA está destinado a:
1.  **Usuarios experimentados** que buscan ahorrar tiempo en despliegues repetitivos.
2.  **Usuarios intermedios** que quieren una guía estructurada mientras mantienen el control de sus archivos de configuración.

> **Nota:** Se recomienda encarecidamente tener abierta la [Gentoo Wiki](https://wiki.gentoo.org/wiki/Handbook:Main_Page) durante el proceso.

## 📁 Estructura del Repositorio

* `setup.sh`: Script principal de orquestación.
* `configs/`: Plantillas de configuración para el sistema y el kernel.
* `scripts/`: Sub-rutinas para tareas específicas (red, usuarios, servicios).

## 📥 Instalación y Uso

1. Inicia desde el Gentoo Minimal LiveCD.
2. Clona este repositorio:
   ```bash
   git clone https://github.com/franjaluga/Gentoo-Deployment-Assistant.git
   
   cd Gentoo-Deployment-Assistant
   ```
Revisa y edita los archivos en configs/ para adaptarlos a tu hardware.

Ejecuta el asistente:

Bash
chmod +x setup.sh
./setup.sh

## 🤝 Feedback
¡Las revisiones de código son bienvenidas! Si encuentras una forma más eficiente de manejar un paso de la instalación o quieres añadir soporte para más perfiles, por favor abre un Issue o un Pull Request.


Disclaimer: Este script realiza cambios permanentes en el disco duro. Úsalo bajo tu propio riesgo.