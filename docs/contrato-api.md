# Contrato de API v1

Detalle completo y ejemplos: guia-integrada.pdf, secciones 7 a 15.
Base local: http://localhost:3000/api. Base MongoDB: tpi_tienda.

- GET/POST /clientes, /productos y /pedidos.
- GET/PATCH/DELETE /clientes/:id, /productos/:id y /pedidos/:id.
- PATCH pedido permite solo estado.
- GET /reportes/ventas-por-categoria y GET /health.
- Lecturas normales: activo=true. DELETE: baja lógica.
- Listados: {data: [], paginacion: {pagina: 1, limite: 10, total: 0}}.
- Individual: {data: recurso}. API usa id string, fechas ISO UTC y centavos enteros.
- Error: {error: {codigo, mensaje, campo}}; campo opcional.
- Pedidos: clienteId e items con productoId/cantidad; precios y total los calcula el servidor.
- Estados: pendiente -> confirmado/cancelado; confirmado -> completado/cancelado.
- Sin cambios de cliente o ítems después de crear.

Documentar aquí solicitudes completas y respuestas reales al implementar.
No cambiar estos contratos sin informar al equipo.
