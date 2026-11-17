---
name: tu-voz
description: >
  Arma el perfil de voz, tono y personalidad de la persona que habla con la IA: no de
  un producto o una marca, sino de ella misma. Responde dos preguntas distintas: cómo
  quiere que la IA le hable y cómo escribe ella cuando la IA escribe en su nombre
  (posts, correos, mensajes, entregables). Parte de la memoria y el historial si
  existen, presenta un borrador para validar y completa lo que falte con una
  entrevista corta. Si no hay historial (cuenta nueva, chat incógnito), empieza
  directo por la entrevista. El resultado es un documento reutilizable. Disparar ante
  frases como "describe mi personalidad", "cuál es mi voz y tono", "quiero que me
  conozcas mejor", "arma mi perfil de voz", "cómo te gustaría que interactuemos",
  "quiero definir cómo hablo", "escribe como yo". Al detectar que aplica, confirmar:
  "¿Armamos tu perfil de voz y tono? Primero reviso qué sé de ti por nuestro
  historial y te lo muestro para validar; lo que falte, te lo pregunto."
---

# Tu voz: perfil de voz, tono y personalidad

Esta skill construye un documento que responde dos preguntas que suelen confundirse:

1. **¿Cómo quiere esta persona que la IA le hable?** (el tono de la IA hacia ella)
2. **¿Cómo habla ella cuando escribe?** (su voz propia, para cuando la IA escribe
   en su nombre: posts, correos, mensajes, entregables)

Son cosas distintas. Alguien puede querer que la IA le hable directo y sin vueltas,
y al mismo tiempo escribir de forma cálida y elaborada. Nunca asumir que son lo mismo.

---

## Protocolo

### Paso 1. Revisar qué contexto existe

Antes de preguntar nada, revisar qué hay disponible:

- **Memoria** (si está activa): cómo pide las cosas la persona, qué corrige seguido,
  en qué tono responde, qué rechaza.
- **Historial de conversaciones** (si hay herramientas para buscarlo): revisar 3 o 4
  conversaciones variadas, no solo la más reciente, para no sacar conclusiones de un
  día atípico.
- **Texto pegado en el chat**: si la persona pega mensajes, posts o correos suyos, es
  la fuente más confiable, porque es texto real y no una impresión de cómo le habla
  a un asistente.

**Si hay memoria o historial:** armar un borrador (Paso 2) y presentarlo para validar,
nunca como definitivo.

**Si no hay nada:** decirlo y pasar directo a la entrevista (Paso 3). No inventar ni
deducir una personalidad a partir de un solo mensaje.

---

### Paso 2. Borrador desde la memoria o el historial

Armar dos bloques separados y presentarlos así:

```
PERFIL BORRADOR, basado en nuestro historial

Cómo te hablo yo a ti (lo que veo en cómo interactúas conmigo):
- [3 o 4 observaciones concretas, con ejemplos reales si se pueden citar]

Tu voz propia (cómo escribes tú, cuando puedo deducirlo):
- [solo si hay evidencia directa: texto tuyo, no una deducción de cómo me hablas a mí]
- Si no hay ejemplos de tu escritura, decirlo: "Todavía no tengo ejemplos de tu
  escritura real. Si me pasas textos tuyos, lo defino mucho mejor."
```

Aclarar siempre: *"Esto es una lectura basada en nuestras conversaciones, no un
análisis riguroso de tu forma de escribir. Si quieres algo más preciso, pásame textos
reales tuyos (posts, correos, mensajes) y lo ajusto contra eso."*

Después del borrador, preguntar: *"¿Esto te representa o hay algo que no encaja?"*
Ajustar según la respuesta antes de pasar al Paso 4.

---

### Paso 3. Entrevista (si no hay historial, o para completar lo que falta)

Un bloque por vez. Esperar la respuesta antes de seguir. Nunca enviar las 10
preguntas juntas.

#### Bloque 1. Cómo quieres que te hable

1. Cuando trabajamos juntos, ¿prefieres que vaya directo al punto o que te dé más
   contexto antes?
2. ¿Te sirve el feedback crítico sin suavizar, o prefieres que lo module?
3. ¿Hay un registro de idioma que prefieras? (por ejemplo: neutro, informal,
   formal, el español de tu país)
4. ¿Hay algo que definitivamente no quieres? (por ejemplo: "no me adules", "no me
   hagas muchas preguntas seguidas", "no repitas lo que ya te dije")

#### Bloque 2. Tu voz propia (cuando escribes tú, o cuando escribo yo por ti)

5. Si tuviera que escribir un mensaje tuyo (a un cliente, en redes, a un colega),
   ¿qué tono debería tener?
6. ¿Hay palabras o expresiones que usas mucho y que te gustaría que aparezcan?
7. ¿Hay palabras, muletillas o estructuras que odias y que nunca deberían aparecer?
8. ¿Tienes algún texto tuyo que puedas pegar aquí? (un correo, un post, un mensaje
   largo). Con eso el análisis deja de ser una impresión y pasa a basarse en tu
   escritura real.

#### Bloque 3. Principios y contexto de fondo

9. ¿Hay algo de tu forma de pensar o de tu historia que atraviesa cómo tomas
   decisiones, más allá del tema puntual?
10. ¿Cómo prefieres recibir información compleja: todo junto o en partes cortas?

---

### Paso 4. Armar el documento final

Con lo validado en el Paso 2 o lo recogido en el Paso 3, construir:

```
## VOZ Y TONO: [Nombre]

### Cómo hablarle (tono de la IA hacia esta persona)
- Registro: [directo / elaborado / neutro / informal / etc.]
- Nivel de feedback: [crítico directo / crítico modulado / diplomático]
- Formato preferido: [respuestas cortas / desarrolladas / por partes]
- Prohibido: [lista concreta, por ejemplo "no adular", "una pregunta por vez"]

### Su voz propia (para lo que se escriba en su nombre)
- Tono: [3 a 5 adjetivos, con qué significa cada uno en la práctica]
- Palabras y expresiones características: [lista, si las hay]
- Palabras o muletillas a evitar: [lista, si las hay]
- Base de este análisis: [impresión general / texto real de la persona]

### Principios de fondo
- [1 a 3 ideas que atraviesan cómo piensa o decide, si surgieron]

### Cómo mantenerlo al día
- Este documento es un punto de partida, no algo cerrado.
- Conviene revisarlo cada tanto: por ejemplo, volviendo a correr esta skill dentro
  de unos meses, o cuando sientas que la IA ya no te habla como necesitas.
```

No prometer que el documento se actualiza solo si no existe un mecanismo real para
hacerlo.

---

### Paso 5. Preguntar cómo guardarlo

No asumir dónde vive el documento. Explicar las opciones en lenguaje simple, sin dar
por hecho que la persona sabe qué es la memoria de la IA:

> "Tu perfil está listo. ¿Cómo quieres guardarlo?
>
> **Opción 1. Que yo lo recuerde:** guardo un resumen en mi memoria, y en las próximas
> conversaciones ya sé cómo hablarte sin que lo repitas.
>
> **Opción 2. Un archivo para ti:** te doy un documento descargable con todo. Puedes
> guardarlo, compartirlo o pegarlo en un chat nuevo cuando no tenga memoria activa
> (por ejemplo, en un chat incógnito o en otra herramienta de IA).
>
> **Opción 3. Las dos cosas.**"

Según lo que elija:

- **Memoria:** guardar un resumen de los puntos clave (las reglas para aplicar, no el
  documento completo).
- **Archivo:** generar un `.md` descargable con el documento del Paso 4.
- **Las dos:** hacer ambas.

Si la memoria no está disponible en su cuenta, decirlo y ofrecer el archivo como
única opción.

---

## Reglas

- **El borrador nunca es definitivo.** Siempre es una hipótesis para validar.
- **Distinguir impresión general de análisis sobre texto real.** Si la persona no pasó
  textos suyos, decirlo en el documento y no dar su voz por definida con la misma
  confianza.
- **No psicoanalizar.** Describir estilo de comunicación y preferencias, nunca rasgos
  clínicos ni motivaciones profundas. Quedarse en lo observable y en lo que la persona
  confirma.
- **Un bloque de preguntas por turno.**
- **Si la persona corrige el borrador,** el documento final refleja la corrección, no
  la primera impresión.
- **Responder en el idioma y el registro de la persona.**
