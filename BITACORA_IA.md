# Bitácora de uso de IA — Grupo 01 · Convocado

Cada entrada registra un prompt dado al agente. Los prompts se copian tal cual fueron enviados.

---

## Entrada N° 1 · Prompt de contexto

- **Fecha y hora:**14/11 a las 3:20hs
- **Integrante:** Silvia Podberezski
- **Aplicación:** Antigravity
- **Modelo:** Claude Sonnet 4.6 (Thinking)
- **Rama de git:** main

### Prompt enviado (literal)
> Contexto del proyecto: estamos construyendo una landing page estática (HTML, CSS y JavaScript vanilla, sin frameworks) para un TP3 de Front End. La landing presenta la startup "Convocado" y DOS propuestas de flujos agénticos, una por cada sentencia asignada. Se revisa solo en desktop.
>
> Reglas de trabajo, obligatorias:
> 1. La landing NO integra IA, no ejecuta agentes, no conecta APIs ni backend. Solo explica y dibuja las propuestas.
> 2. Las sentencias originales NO se pueden reescribir, resumir ni reordenar. Deben copiarse tal cual están en el archivo fuente/asignacion.md.
> 3. Distinguir siempre lo que dice la sentencia (etiqueta "Obligatorio Sentencia", verde) de lo que agrega el grupo (etiqueta "Decisión Diseño Grupo", ámbar punteado). Si algo no está escrito en la sentencia, es decisión del grupo.
> 4. No inventes datos, nombres, funciones ni integrantes. Si te falta información, preguntame.
> 5. Modificá SOLO los archivos que te nombre en la tarea. No toques otros archivos ni cambies estructura, estilos o contenido que no te pedí.
> 6. Los desplegables usan <details>/<summary> y deben funcionar con clic y teclado.
> 7. No debe haber desborde horizontal en desktop (1440 px).
>
> Antes de modificar cualquier archivo: leé los archivos relevantes, mostrame un plan breve con los archivos que vas a tocar y qué cambiarías en cada uno, y esperá mi aprobación. Al terminar, listá exactamente qué archivos modificaste y qué cambió en cada uno.

### Qué hizo el agente
Leyó los archivos del proyecto (index.html, styles.css, diagramas.html, diagramas.css, script.js y el análisis funcional) y resumió su estado. No modificó nada y pidió que le indicara una tarea. Llamó "Fuente/asignacion.md" al archivo analisis_funcional_convocado_grupo01.md, porque el archivo fuente/asignacion.md todavía no existía.

### Archivos modificados
- Ninguno.

### Cómo lo verificamos
Antes de este prompt, le pedí que listara los archivos del proyecto y comprobé que nombrara los archivos esperados (index.html, diagramas.html, styles.css, diagramas.css, script.js, README.md, analisis_funcional_convocado_grupo01.md y la carpeta assets), para confirmar que estaba trabajando en la carpeta del repositorio clonado y no en otro proyecto.

### Problema detectado (si lo hubo)
La confusión de nombre indicada arriba. No tuvo consecuencias.

### Prompt de corrección (literal)
No hizo falta.

### Resultado final
El agente quedó con el contexto y las reglas de trabajo, sin tocar archivos.

### Commit
Sin commit (no hubo cambios).

---

## Entrada N° 2 · Tarea 0: archivo fuente con las sentencias

- **Fecha y hora:** 14/11 a las 4:00hs
- **Integrante:** Silvia Podberezski
- **Aplicación:** Antigravity
- **Modelo :** Claude Sonnet 4.6 (Thinking)
- **Rama de git:** main

### Prompt enviado (literal)
> Creá el archivo fuente/asignacion.md con exactamente este contenido, sin cambiar ni una palabra, ni signos de puntuación:
>
> # Asignación del Grupo 01
>
> - Startup: Convocado
> - Categoría: Deportes y conexión de equipos
> - Objetivo de la startup: Red para que jugadores encuentren equipos y soliciten participar en partidos.
> - Bloque: Cupo y revisión
> - Código de asignación: S08-B
> - Origen: startup creada por estudiantes del IFTS 16; propuesta realizada por el Grupo 01 del IFTS 29.
>
> ## Frase 1 · R3
> Si el capitán intenta aceptar una solicitud cuando ya no queda lugar, el sistema informa que el cupo está completo e impide una nueva aceptación.
>
> ## Frase 2 · R4
> Si el jugador autoriza una solicitud y se cumple al menos una de estas condiciones —su valoración conocida es menor que cuatro, o el equipo está a diez kilómetros o más—, el sistema la deriva al capitán para evaluación manual; esa evaluación no reserva un lugar.
>
> No modifiques ningún otro archivo.

### Qué hizo el agente
Mostró un plan (crear un solo archivo nuevo dentro de una carpeta fuente/ inexistente), se respondió solo "¿Procedo? Sí" sin esperar mi aprobación y creó fuente/asignacion.md.

### Archivos modificados
- fuente/asignacion.md (nuevo)

### Cómo lo verificamos
Comparé el contenido del archivo con el texto de la consigna en PDF, palabra por palabra: la Frase 1 y la Frase 2 coinciden, incluidas las rayas largas (—), el "su valoración conocida" y el punto y coma. Corrí git status: solo apareció fuente/ como archivo nuevo, sin otros archivos modificados.

### Problema detectado (si lo hubo)
El agente ejecutó sin esperar mi aprobación, aunque el prompt de contexto se la pedía. No causó daño porque la tarea era crear un archivo nuevo.

### Prompt de corrección (literal)
No hizo falta.

### Resultado final
El archivo fuente/asignacion.md quedó creado con las sentencias exactas, como fuente de verdad para las demás tareas.

### Commit
Pendiente (se hará junto con la bitácora).

---

## Entrada N° 3 · Tarea 0: creación de la bitácora

- **Fecha y hora:** 14/11 a las 4:20
- **Integrante:** Silvia Podberezski
- **Aplicación:** Antigravity
- **Modelo :** Claude Sonnet 4.6 (Thinking)
- **Rama de git:** main

### Prompt enviado (literal)
> Creá el archivo BITACORA_IA.md en la raíz del proyecto con este contenido exacto, sin agregar nada:
>
> # Bitácora de uso de IA — Grupo 01 · Convocado
>
> Cada entrada registra un prompt dado al agente. Los prompts se copian tal cual fueron enviados.
>
> ---

### Qué hizo el agente
Mostró un plan (crear un solo archivo en la raíz) y volvió a ejecutar sin esperar mi aprobación. Creó BITACORA_IA.md con el contenido indicado.

### Archivos modificados
- BITACORA_IA.md (nuevo)

### Cómo lo verificamos
Abrí el archivo con el Bloc de notas y comprobé que el contenido coincide con el prompt, sin líneas agregadas.

### Problema detectado (si lo hubo)
Otra vez ejecutó sin esperar la aprobación. A partir de este punto empiezo cada prompt con la indicación de mostrar solo el plan y esperar mi "Aprobado".

### Prompt de corrección (literal)
No hizo falta.

### Resultado final
La bitácora quedó creada y lista para registrar el resto de los prompts.

### Commit
Pendiente (se hará junto con fuente/asignacion.md).
