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

## Gestión de Usuarios

El sistema permite una administración completa del ciclo de vida del usuario:

- Alta de Usuario

- Creación automática con useradd

Asignación dinámica de grupos según el puesto:

- vendedor / cajero → ph_ventas

- gerente → ph_admin, ph_ventas

- sistemas → ph_admin, ph_soporte

- Configuración de fecha de caducidad

- Creación de directorio home

- Asignación obligatoria de contraseña

- Registro automático en archivo de logs

- Baja de Usuario

- Eliminación opcional del directorio home

- Registro del evento administrativo

- Consulta

Muestra:

- Información del usuario (finger)

- Grupos asociados

- Fecha de expiración

- Procesos activos

- Último login

Modificación que permite:

- Cambiar fecha de caducidad

- Modificar directorio home

- Bloquear/desbloquear cuenta

- Cambiar grupo principal

- Actualizar puesto
