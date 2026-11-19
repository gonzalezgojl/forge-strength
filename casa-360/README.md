# CASA 360

PWA para organizar el mantenimiento del hogar desde el iPhone.

## Funciones
- Crear tareas propias y organizarlas por zonas personalizables.
- Repetición cada cierto número de días, semanas o meses.
- Fecha prevista, prioridad, instrucciones y foto de referencia.
- Materiales y herramientas asociados a cada tarea.
- Lista de compras automática, con cantidades, fotos y enlaces de producto.
- Registro de reparaciones, gastos, facturas y tickets.
- Historial de tareas completadas y reparaciones resueltas.
- Exportación e importación de copia JSON.
- Instalable como aplicación web progresiva y shell básico sin conexión.

## Datos y privacidad
Los datos, fotos y documentos se guardan localmente en IndexedDB del navegador/dispositivo. No se envían a GitHub ni a un servidor. No hay cuentas ni sincronización entre dispositivos. Exporta una copia periódicamente y antes de cambiar de dispositivo o navegador.

## Avisos
La app muestra tareas pendientes y atrasadas cuando se abre. Puede intentar mostrar notificaciones mientras la app está abierta y ejecutándose, si el navegador lo permite. En iPhone primero hay que añadir la PWA a la pantalla de inicio y conceder permiso. Las notificaciones que lleguen con la app cerrada requieren un servicio Web Push y un servidor que envíe los mensajes; GitHub Pages por sí solo no las programa ni las envía. El service worker incluye el receptor para una futura configuración Web Push.

## Publicación
Ruta prevista:
https://gonzalezgojl.github.io/forge-strength/casa-360/

Si GitHub Pages no está activado:
1. Abre el repositorio gonzalezgojl/forge-strength en GitHub.
2. Settings → Pages.
3. Elige Deploy from a branch.
4. Branch main y carpeta /(root), y guarda.

## Instalar en iPhone
1. Abre la URL anterior en Safari.
2. Pulsa Compartir.
3. Selecciona Añadir a pantalla de inicio.
4. Activa Abrir como app si aparece y pulsa Añadir.
5. Abre CASA 360 desde el nuevo icono.
