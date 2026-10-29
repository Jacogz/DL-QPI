# NEXT

Actualizado: 2026-10-29
Issue activo: ninguno fijo — #7, #8, #9 abiertos (ver Estado)

## Siguiente paso
- Pendiente de una próxima sesión: adjuntar e indexar el documento de entregable #1 (título +
  objetivo general + específicos, ya enviado) en `docs/` y actualizar el README con la sección
  "Objetivos" (issue #4 se cerró ya, pero el DoD original —README actualizado— no se cumplió
  todavía; queda como deuda a resolver cuando llegue el documento).
- #9 (Jacobo): ADR de arquitectura general del pipeline — buen punto de partida porque #7 y #8
  dependen de cómo queden definidas las interfaces entre componentes.
- #7 (sin asignar — Juan aún no es colaborador del repo): limpieza de datasets (malaria y fases
  RBC).
- #8 (Sahian): heurística de validación (segmentación + perfil/delta de fase).
- #6 sigue abierto: setup del entorno en el notebook de Colab, sin definir.

## Estado
Sesión del 2026-10-29 (post-reunión del profesor, 2026-10-28):
- **#3** cerrado — `docs/reunion-2026-10-28.md` committeado, con las 3 opciones de problema y las
  respuestas del profesor a las preguntas abiertas. Dirección elegida: opción 3 (bridge CycleGAN
  malaria→fase, usando la reconstrucción de eritrocitos sanos como base técnica).
- **#5** cerrado — tabla de roles agregada al README (documentación, no división rígida de
  trabajo; los 3 pueden tocar cualquier parte): Jacobo=arquitectura, Juan=datos, Sahian=heurística
  /modelo.
- **#4** cerrado — entregable #1 (título + objetivo general + específicos) ya enviado al
  profesor. Falta adjuntar el documento al repo e indexarlo (ver Siguiente paso).
- **#7, #8, #9** creados y agregados al Project 6, detallando las tareas iniciales de la nueva
  dirección (limpieza de datos, heurística de validación, ADR de arquitectura).

Pipeline acordado para la limpieza de malaria (issue #7): RGB→gris → rescale para igualar tamaño
de célula → recorte 256x256 → eliminar imágenes (menos de 3 células / con infección / con cúmulos
difíciles de segmentar) → aumentación (flips y rotaciones aleatorias). Para fases RBC: eliminar
imágenes con manchas oscuras.

Heurística de validación (issue #8): segmentar eritrocitos en imágenes de fase, calcular perfil y
delta de fase por eritrocito, visualizar la reconstrucción de cada uno, y anotar sobre la imagen
completa el promedio de perfil/delta por imagen.

## Bloqueos y dudas
- Juan (`juanlotero2552`) no es colaborador del repo todavía — issue #7 quedó sin asignar hasta
  que acepte una invitación.
- Setup del entorno en el notebook de Colab sin definir (issue #6).
- Deuda del DoD original de #4: el README no tiene todavía la sección "Objetivos" con el
  contenido enviado al profesor (se resuelve cuando se adjunte el documento).
