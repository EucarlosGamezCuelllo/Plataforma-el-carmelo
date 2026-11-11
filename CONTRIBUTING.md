# Convenciones de trabajo

## Ramas
- `main`: rama estable. Solo recibe cambios que cumplen la definición de terminado.
- `feature/HUxx-descripcion`: una rama por historia de usuario. Ejemplo: `feature/HU03-descarga-offline`.
- `fix/descripcion`: correcciones de defectos.

## Mensajes de commit
Formato: `tipo(HUxx): descripción corta` y, en el cuerpo, el sprint.

Tipos: `feat`, `fix`, `docs`, `test`, `chore`, `refactor`.

Ejemplos:
```
feat(HU03): habilitar descarga de contenidos en Moodle App
test(PF-05): registrar resultado de consulta sin conexión
docs(manual): agregar guía para crear un curso desde la plantilla
```

## Definición de terminado
1. Cumple los criterios de aceptación de su historia de usuario.
2. Superó las pruebas funcionales y de acceso desde el celular.
3. Fue revisado por el director del proyecto o por el dueño del producto.
4. Está documentado en la guía de configuración o en el manual de usuario.
5. Se desplegó en el entorno de pruebas sin errores críticos pendientes.

## Incidencias (issues)
Cada defecto se registra con severidad (crítica, mayor, menor), pasos para reproducirlo y el ID de la prueba.
Un defecto crítico abierto impide cerrar el sprint.

## Lo que nunca se sube
Contraseñas, claves, `config.php`, respaldos con usuarios y datos personales de estudiantes.
