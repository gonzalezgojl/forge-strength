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
- Exportación de cada tarea como evento iCalendar (.ics), con repetición y aviso para añadirlo al calendario del móvil.
- Instalable como aplicación web progresiva y shell básico sin conexión.

## Datos y privacidad
Los datos, fotos y documentos se guardan localmente en IndexedDB del navegador/dispositivo. No se envían a GitHub ni a un servidor. No hay cuentas ni sincronización entre dispositivos. Exporta una copia periódicamente y antes de cambiar de dispositivo o navegador.

## Avisos
La app muestra tareas pendientes y atrasadas cuando se abre. Puede intentar mostrar notificaciones mientras la app está abierta y ejecutándose, si el navegador lo permite. En iPhone primero hay que añadir la PWA a la pantalla de inicio y conceder permiso. Para recibir avisos aunque CASA 360 esté cerrada, puedes exportar cada tarea a un archivo iCalendar (.ics) e importarlo en el calendario del móvil; el calendario del sistema gestionará sus alertas. En iPhone, Apple documenta la importación de archivos .ics desde Mail y la suscripción a calendarios .ics. Las notificaciones propias de CASA 360 con la app cerrada requieren un servicio Web Push y un servidor que envíe los mensajes; GitHub Pages por sí solo no las programa ni las envía. El service worker incluye el receptor para una futura configuración Web Push.

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

## Plano interactivo de la vivienda
Se han incorporado las dos plantas aportadas: planta superior y garaje/gimnasio. Las zonas pulsables enlazan con las zonas de las tareas. El color es local: rojo para tareas vencidas, amarillo para tareas que vencen en 7 días o menos, verde para tareas programadas más adelante y gris cuando no hay tareas activas. Los planos se incluyen como recursos locales y se precargan en el service worker.
