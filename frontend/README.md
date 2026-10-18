# Frontend · TPI Tienda

Prototipo de tienda desarrollado con React, TypeScript, Vite, Tailwind CSS y shadcn/ui a partir del mockup HTML del equipo. Funciona con datos ficticios en memoria; al recargar, vuelve al estado inicial. La integración con la API Express está pendiente.

## Ejecutar

Requiere Node.js compatible con Vite 7 (20.19+ o 22.12+).

```powershell
cd frontend
npm install
npm run dev
```

Abrir `http://localhost:5173`. Para comprobar la compilación de producción: `npm run build`.

## Estructura

| Ruta | Responsabilidad |
| --- | --- |
| `src/app.tsx` | Composición de secciones y estado de navegación |
| `src/pages/` | Pantallas de resumen, clientes, productos, pedidos y reportes |
| `src/components/ui/` | Componentes generados por shadcn/ui |
| `src/components/common/` | Piezas visuales reutilizables |
| `src/components/forms/` | Formularios de entidades y pedidos |
| `src/components/orders/` | Detalle histórico del pedido |
| `src/mocks/` | Datos de demostración y reglas de negocio del mock |
| `src/lib/constants/` | Categorías, estados, navegación y paginación |

La [guía de estilos](DESIGN.md) registra colores, tipografía y patrones. Las [reglas de trabajo](AGENTS.md) establecen convenciones para los siguientes cambios.

## Alcance del prototipo

- Listados, filtros y paginación de clientes, productos y pedidos.
- Altas y edición de clientes y productos, con baja lógica.
- Creación de pedidos, detalle con datos históricos y cambios válidos de estado.
- Reporte de ventas por categoría con filtro de fechas.
- Validaciones básicas y mensajes de éxito/error en los formularios.

Los identificadores mock tienen formato de 24 caracteres hexadecimales para ser compatibles con el contrato de la API. La implementación actual no realiza solicitudes HTTP. `VITE_API_URL` está preparada en `.env.example` para la integración posterior.
