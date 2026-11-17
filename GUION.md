# Guion · Cómo controlar una IA que nos supere

**Duración estimada:** 12 minutos + preguntas.
**Orador:** Augusto Traverso (5° E · TEI 2026).
Las acciones van **[entre corchetes]**. Las mismas notas están en la presentación (tecla **N**).

| # | Diapositiva | Tiempo | Acumulado |
|---|---|---|---|
| 1 | Portada | 0:45 | 0:45 |
| 2 | Un caso hipotético | 1:00 | 1:45 |
| 3 | Mi hipótesis | 1:30 | 3:15 |
| 4 | Capacidad y autonomía | 1:00 | 4:15 |
| 5 | Tres problemas | 0:45 | 5:00 |
| 6 | Dónde aparecen los riesgos (5 pasos) | 1:15 | 6:15 |
| 7 | Supervisar algo más capaz (3 pasos) | 1:30 | 7:45 |
| 8 | AI Control (4 pasos) | 1:30 | 9:15 |
| 9 | La entrevista | 0:45 | 10:00 |
| 10 | Defensa en profundidad (4 pasos) | 0:45 | 10:45 |
| 11 | Qué pasó con mi hipótesis | 0:45 | 11:30 |
| 12 | Conclusión | 0:30 | 12:00 |
| 13 | Fuentes | — | (solo si preguntan) |

---

## 1 · Portada (0:45)

[Abrir con Enter; la cámara baja hasta la escena.]

> Mi tesina parte de una pregunta: **¿sería posible mantener bajo control humano un sistema que supere a las personas en la mayoría de las tareas cognitivas?** Es decir, una AGI.
>
> Les presento la imagen que nos va a acompañar toda la charla. El poliedro violeta es la IA. La esfera cálida es quien la supervisa, y el cono de luz es lo que llega a revisar. Las chispas que salen de la IA son sus acciones: las verdes las detectamos; las rojas se escapan.

## 2 · Un caso hipotético (1:00)

> Imaginen esto. Una IA escribe un programa que ninguna persona del equipo entiende por completo. Las pruebas habituales dan bien y el sistema recomienda usarlo.

[Hacer clic en **Aprobar**.]

> Listo, aprobado. Pero, ¿esto es control humano o es solo una firma?
>
> Esta duda me quedó después del seminario de IA de la escuela. Me interesó menos imaginar qué podría hacer una inteligencia superior que entender cómo revisaríamos sus decisiones. Aclaro algo: no doy por hecho que una AGI vaya a existir ni predigo cuándo. Analizo esa posibilidad con investigaciones sobre sistemas actuales.

## 3 · Mi hipótesis (1:30)

[Leer la hipótesis despacio.]

> Mi hipótesis es que, si aumenta la diferencia de capacidad entre la IA y quienes la supervisan, y además recibe más autonomía, la supervisión directa va a detectar una proporción menor de fallas, **siempre que los recursos de supervisión sean los mismos.**

[Subir de a poco los dos controles: la IA crece fuera del cono y aparecen más chispas rojas.]

> Esto es una simulación ilustrativa de lo que predice la hipótesis; no son datos medidos.
>
> ¿Qué me haría cambiar de idea? Experimentos reproducibles en los que la detección se mantenga al aumentar esas dos variables, con una utilidad razonable. Bloquear todo evitaría riesgos, pero también impediría aprovechar el sistema.
>
> Para ponerla a prueba comparé experimentos sobre supervisión y control, una propuesta de Google DeepMind y una entrevista publicada a un investigador de Redwood Research. No hice experimentos propios.

[Volver los controles al mínimo antes de avanzar (opcional).]

## 4 · Capacidad y autonomía (1:00)

> Primero, las definiciones. Llamo AGI a un sistema que iguala o supera el desempeño humano en una amplia variedad de tareas cognitivas. El marco *Levels of AGI*, de Morris y colegas, separa dos cosas: qué tan capaz es y cuánta autonomía tiene.

[Señalar la grilla: la altura es la capacidad y el color, la autonomía.]

> El sistema A es muy capaz, pero solo recomienda. El B es menos capaz, pero puede modificar archivos sin preguntar. Por eso la diferencia importa.
>
> Entonces, ¿qué es "control humano"? Que las personas puedan **fijar objetivos, limitar accesos, detectar desviaciones y detener acciones peligrosas.** Tiene que haber una posibilidad real de intervenir, no solo una aprobación formal.

## 5 · Tres problemas (0:45)

> Hay tres palabras que se confunden. El **alineamiento** busca que el sistema actúe según nuestras intenciones. El **AI Control** estudia cómo impedir daños aunque el alineamiento falle. Y el **superalignment** lleva el alineamiento a sistemas que superarían ampliamente a sus supervisores. Están relacionados, pero no son intercambiables.

## 6 · Dónde aparecen los riesgos (1:15) · 5 pasos

[Cada → abre una grieta en el escudo.]

1. > **Objetivos incompletos.** Si le pido reducir costos, podría recomendar eliminar revisiones de seguridad. Es un ejemplo hipotético.
2. > **Convincente no es correcto.** Que el código pase las pruebas no garantiza que funcione con cualquier entrada. Si no detecto el error, mi aprobación protege poco.
3. > **Acciones irreversibles y rápidas.** Borrar información, publicar datos privados o tocar infraestructura antes de que alguien pueda intervenir.
4. > **Evasión deliberada.** Se investiga con modelos instruidos para introducir fallas. Eso sirve para probar defensas, pero no demuestra que una IA vaya a hacerlo sola.
5. > **Aprobar por costumbre.** Acostumbrarnos a aceptar sin mirar. Esta es una preocupación mía, no un resultado medido.

## 7 · Supervisar algo más capaz (1:30) · 3 pasos

> ¿Qué pasa cuando el supervisor es menos capaz? Hay tres líneas de investigación.

1. [La cámara va a la maqueta "asistencia".]
   > **Bowman y colegas (Anthropic, 2022):** las personas asistidas por un modelo poco confiable superaron al modelo solo y a las personas sin ayuda. Pero eran tareas de preguntas y respuestas, no acciones de una AGI.
2. [Maqueta "débil → fuerte".]
   > **Burns y colegas (OpenAI, 2023):** entrenaron un modelo fuerte con las respuestas de uno débil. El fuerte superó a su supervisor y recuperó parte de su capacidad, aunque no toda. Aprender bien en una prueba no es lo mismo que actuar según nuestros objetivos.
3. [Maqueta "debate".]
   > **Kenton y colegas (2024):** dos modelos defienden respuestas distintas ante un juez. El debate le ganó a consultar a un modelo, pero frente a responder directo dependió de la tarea. No es una solución universal.

## 8 · AI Control (1:30) · 4 pasos

> El trabajo más cercano a mi pregunta es el de Greenblatt y colegas (2024). GPT-4, que no es confiable, escribe código; GPT-3.5, que sí lo es, lo revisa; y hay una auditoría limitada. Los investigadores preparan a GPT-4 para que intente esconder fallas.

[Señalar la cinta: los bloques violetas son código y la puerta verde es el monitor.]

1. > **Auditoría inicial:** la utilidad es completa, pero la seguridad es de solo 15.
2. > **Monitoreo confiable:** GPT-3.5 marca lo sospechoso. La seguridad sube a 62.
3. > **Derivación:** el 20 % más sospechoso lo reescribe GPT-3.5. La seguridad llega a 92, pero la utilidad baja a 83.
4. > **Edición:** en vez de descartar ese código, se corrige. Seguridad 92 y utilidad 94.

> Dos aclaraciones. La seguridad es la probabilidad de completar 5000 problemas simulados sin aceptar una falla oculta, y la utilidad está reescalada entre GPT-3.5 y GPT-4. No es una garantía sobre una AGI. Queda abierto cuánto se mantendría con tareas nuevas y atacantes más capaces.

## 9 · La entrevista (0:45)

> Para escuchar a un especialista, usé la entrevista de Rob Wiblin a Buck Shlegeris en el podcast 80,000 Hours. No es una entrevista mía.
>
> En el minuto 33:18 explica que una propuesta sospechosa puede descartarse y reemplazarse antes de ejecutarse, que es lo que se ve en la puerta. En el 1:01:05 aparece otra dificultad: que las empresas apliquen realmente las medidas.
>
> Un detalle: Shlegeris es coautor del paper, así que su testimonio no es una validación independiente.

## 10 · Defensa en profundidad (0:45) · 4 pasos

[Cada → suma una capa alrededor de la IA.]

> Google DeepMind propone en su AI Control Roadmap, de 2026, combinar varias defensas: alineamiento, monitoreo, restricción de accesos y respuesta. Si una falla, otra todavía puede intervenir. También separa lo reversible, que se puede revisar después, de lo irreversible, que hay que bloquear antes.
>
> Pero una hoja de ruta es una propuesta, no una demostración experimental.

## 11 · Qué pasó con mi hipótesis (0:45)

> Mi hipótesis no quedó confirmada ni refutada: quedó **matizada.** Es compatible con los límites que muestran los estudios, pero no encontré ninguno que varíe capacidad y autonomía por separado con los mismos recursos. Además, la asistencia, el debate y la revisión compensan la brecha en algunas condiciones.
>
> Tampoco junto porcentajes de trabajos distintos, porque miden cosas diferentes. Para probarla de verdad haría falta el experimento que está abajo.

## 12 · Conclusión (0:30)

> Mi respuesta es que mantener el control parece posible bajo ciertas condiciones. No está garantizado para una AGI en cualquier contexto, y perderlo tampoco es inevitable.
>
> Antes pensaba solo en la diferencia de inteligencia. Ahora creo que importa más cómo organizamos la supervisión. Mi postura es que **la autonomía debería depender de la evidencia de control.**
>
> Y me queda una pregunta: **¿qué decisiones estamos dispuestos a delegar mientras todavía aprendemos a supervisarlo?** Gracias. ¿Preguntas?

---

## Preguntas probables

**¿Entonces creés que la AGI va a existir?**
No lo doy por hecho ni predigo cuándo. Analizo la posibilidad con lo que se puede estudiar hoy.

**¿Por qué no hiciste tu propio experimento?**
Para probar la hipótesis hace falta variar capacidad y autonomía con modelos y presupuestos comparables. Eso está fuera del alcance de una tesina. Por eso comparé estudios y aclaro qué permite concluir cada uno.

**¿Qué diferencia hay entre alineamiento y control?**
El alineamiento busca que el sistema *quiera* lo mismo que nosotros. El control busca que no pueda hacer daño *aunque* no lo quiera.

**Si el debate y la asistencia funcionan, ¿tu hipótesis es falsa?**
No del todo. Mi hipótesis habla de supervisión *sin cambios en los recursos*, y esas técnicas agregan herramientas. Sí cuestionan que superar al supervisor implique volverse incontrolable.

**¿Por qué no sumás los resultados de todos los estudios?**
Porque miden cosas diferentes: aprender de etiquetas imperfectas, elegir la respuesta correcta y evitar código con fallas ocultas.

**¿Usaste IA para la tesina?**
Sí. Usé ChatGPT para investigar fuentes y asistir la redacción, y el gráfico se armó con asistencia de IA a partir de la tabla 7 del paper.

**¿Qué significa "utilidad reescalada"?**
0 es el desempeño de GPT-3.5 y 100, el de GPT-4. No es un porcentaje de código correcto.

## Antes de presentar

- Probarla en la computadora del aula con Chrome o Edge **y con internet** (carga three.js, GSAP y las fuentes desde la web).
- Revisar que el link del episodio (diapositiva 9) abra la página correcta.
- Tecla **F** para pantalla completa; **N** para ver estas notas; **1–9 / 0** para saltar a una diapositiva.
