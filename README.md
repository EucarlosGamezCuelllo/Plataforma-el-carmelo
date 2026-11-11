# Plataforma digital de aprendizaje – I.E. El Carmelo

Prototipo funcional (TRL 5) de una plataforma de aprendizaje basada en **Moodle** (software libre) para apoyar la
transición de la enseñanza tradicional hacia entornos digitales en la Institución Educativa El Carmelo de
San Juan del Cesar, La Guajira.

- **Autor:** Eucarlos Gámez Cuello
- **Tutor:** Orlando Gómez Barboza
- **Curso:** Proyecto de grado 202016907_5 – Programa de Ingeniería de Sistemas, UNAD
- **Metodología:** Scrum + ADDIE, dentro de la iniciativa CDIO
- **Plataforma en línea:** `[COMPLETAR: URL]`
- **Video demostrativo (máx. 10 min):** `[COMPLETAR: enlace]`

## Qué contiene este repositorio

| Carpeta | Contenido |
|---|---|
| `docs/` | Documento maestro, arquitectura y diseño, guía de instalación, manual de usuario, requisitos y guía de transición |
| `moodle-config/` | Complementos, ajustes, script de instalación del servidor y ejemplo de configuración (sin claves) |
| `theme/` | Tema con la identidad institucional |
| `courses/` | Copias de respaldo `.mbz` del curso plantilla y de los cursos (sin datos de usuarios) |
| `h5p/` | Contenidos interactivos `.h5p` |
| `scripts/` | Respaldo, restauración y plantilla de carga masiva de usuarios |
| `tests/` | Casos de prueba, resultados, métricas y evidencias |

## Requisitos del servidor

- Linux (Ubuntu Server LTS recomendado), Apache o Nginx
- PHP (versión compatible con la versión de Moodle) y extensiones requeridas
- MariaDB o MySQL
- Dominio y certificado SSL/TLS
- Moodle (versión estable con soporte de largo plazo): `[COMPLETAR: versión instalada]`

## Instalación resumida

1. Preparar el servidor: `sudo bash moodle-config/instalar_servidor.sh`
2. Completar el asistente web de Moodle (ver `docs/guia_instalacion.md`).
3. Aplicar los ajustes de `moodle-config/ajustes.md`.
4. Restaurar los cursos de `courses/` y los contenidos de `h5p/`.
5. Configurar la copia de respaldo diaria con `scripts/respaldo.sh`.

## Metodología y trazabilidad

El trabajo se organiza en sprints de dos semanas. Cada historia de usuario (HU) se desarrolla en una rama
`feature/HUxx-descripcion` y se integra a `main` al cumplir la definición de terminado. Ver
[`CONTRIBUTING.md`](CONTRIBUTING.md) y `docs/requisitos.md`.

## Pruebas

Casos y resultados en `tests/`. Meta: ≥ 90 % de pruebas funcionales superadas, SUS ≥ 68, TAM favorable ≥ 70 %.

## Privacidad

Este repositorio **no** contiene contraseñas, claves ni datos personales de estudiantes (menores de edad).
Ver `.gitignore`.

## Licencia

Documentación bajo CC BY 4.0. Los scripts propios se publican bajo licencia MIT. Moodle y H5P conservan sus
licencias originales (GPL v3 y MIT, respectivamente).
