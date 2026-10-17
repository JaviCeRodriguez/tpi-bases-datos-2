# TPI - Bases de Datos 2

Tienda de prueba con clientes, productos y pedidos en MongoDB Atlas.

| Integrante | Responsabilidad |
| --- | --- |
| Matías Yacob | Modelo, Atlas, backend Express, validaciones, índices y reporte |
| Javier | Frontend React + Vite e integración con la API |
| Brenda | Respaldos PowerShell, programación y restauración |

La guía integrada en `docs/guia-integrada.pdf` es el contrato inicial del grupo.
Todos documentan su parte y deben poder explicar el sistema completo.

## Estado inicial

Este repositorio contiene la estructura y la documentación para iniciar el trabajo.
La aplicación, los scripts y las pruebas todavía no están implementados.

## Trabajo en equipo

Crear ramas por tarea, por ejemplo `matias/backend`, `javier/frontend` y
`brenda/respaldos`. Integrar mediante pull requests revisados por otro integrante.
Matías revisa respaldo, Brenda frontend y Javier modelo/backend.
Comunicar cambios de contratos antes de integrarlos.

## Configuración y secretos

No subir URI con credenciales, archivos .env reales ni respaldos.
Las plantillas .env.example muestran variables sin secretos.
La base acordada es tpi_tienda. La restauración se prueba en
tpi_tienda_restore_test. Usar solo datos ficticios.
