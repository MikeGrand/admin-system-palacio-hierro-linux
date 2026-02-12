# admin-system-palacio-hierro-linux
Palacio de Hierro – Versión 3.0

Este proyecto consiste en un script avanzado en Bash diseñado para la administración integral de infraestructura Linux dentro de un entorno empresarial simulado del Palacio de Hierro.

El sistema automatiza tareas críticas de administración como:

- Gestión de usuarios y grupos

- Programación de tareas automáticas

- Respaldos y recuperación de información

- Administración de bases de datos

- Monitoreo de red y seguridad

- Integración con herramientas profesionales (Nagios, Nmap, Wireshark, rsync, cron, at)

El objetivo del proyecto es centralizar funciones administrativas en una interfaz estructurada por menús, permitiendo una gestión eficiente, segura y organizada del sistema.

## Arquitectura y Configuración

El script establece una estructura organizacional basada en departamentos:

- Ventas

- Inventario

- Sistemas

Define rutas y variables base como:

- Directorios administrativos (/ph/departamento)

- Carpeta de respaldos (/backups/ph_departamento)

- Archivo de logs (/var/log/ph_admin.log)

- Configuración MySQL

- Dominio empresarial (ph.local)

Además, valida que el script sea ejecutado únicamente por el usuario root, garantizando permisos adecuados para operaciones críticas del sistema.
