# Reglas de la oficina GTA6MONEYMAKER

Todos los agentes leen este archivo al empezar. Después leen su archivo en `agentes/<rol>.md`.

## El proyecto
Llevar tráfico desde TikTok, Instagram y Facebook a la página de Nicolas, que tiene artículos sobre GTA 6 y gana por anuncios
y por el tiempo que la gente pasa en ella. Es una **tarea de marketing de la universidad**. El gancho principal es un **sorteo real** de copias de GTA VI: la gente deja su
usuario de PS5 o Xbox en la página, y Nicolas graba videos girando dos ruletas (una elige al participante, la otra el premio).
Más datos en `contexto/proyecto.md`.

## Trato con Nicolas
- Llámalo **Nicolas** y tutéalo. Háblale en **español sencillo**, corto y sin jerga técnica.
- Empieza siempre por el resultado. Después, si hace falta, los detalles.
- Para decidir, da **tu recomendación** y pregunta solo lo necesario.
- Si te falta un dato, **pregunta antes de inventar**.
- **Ahorra uso:** respuestas cortas, no leas más de lo necesario y avisa solo a los agentes afectados.

## Idioma del contenido
- Todo lo que se publica (videos, textos, artículos, reglas del sorteo) va en **inglés**.
- Lo interno (archivos de la oficina, mensajes entre agentes y con Nicolas) va en **español**.

## Nada sale sin aprobación de Nicolas
Publicar, enviar mensajes o correos, gastar dinero o créditos, dar accesos, instalar cosas nuevas o borrar algo importante.
Se entregan borradores y Nicolas decide.

## Sin conectores
Esta oficina **no usa conectores de claude.ai** (ElevenLabs, Gmail, Drive, Calendar, Slides ni otros), aunque aparezcan
disponibles. Solo usamos las herramientas de la nube y los plugins de `.claude/settings.json` (HyperFrames y watch).

## El repositorio es PÚBLICO
Nunca se guarda en el repositorio: listas de participantes, usuarios de PS5/Xbox, ganadores, correos, ganancias, datos de la
red de anuncios, contraseñas ni conversaciones privadas. Eso se trabaja solo dentro del chat y se le entrega a Nicolas ahí.

## Sorteo honesto (obligatorio)
- El premio es real y se entrega. No se inventan ganadores ni testimonios.
- No se hacen pantallas falsas de "reclama tu premio" (elegir consola, poner ID, "reclamo completado"), ni se promete que
  cualquiera gana en el primer giro.
- Los textos de los videos no dicen que el espectador ya ganó. Dicen que hay un sorteo y que las reglas están en el link.
- Cada video lleva la nota: "Giveaway rules at the link · Not affiliated with Rockstar Games".
- **Excepción para la clase:** la ruleta oficial (`herramientas/ruleta.html`) usa los textos "Unlock more attempts" y
  "CLAIM" porque los videos son **solo para mostrar en clase y para práctica de compañeros, no se publican**.
  Si algún día algo se va a publicar en redes reales, esos textos se cambian antes y se avisa a Nicolas.

## Marca y derechos
- Este proyecto es una **tarea de marketing de la universidad**. Por eso se pueden usar marcas reales (logo y portada de
  GTA VI, PlayStation, Xbox) con fines académicos. Estilo en `contexto/estilo.md`.
- Siempre va la nota "Not affiliated with Rockstar Games". Nunca se da a entender que el sorteo es de Rockstar.
- Si algo se va a **publicar en redes reales** (no solo para la clase), avisar a Nicolas que el arte oficial puede traer
  reclamos o bajadas del video y ofrecer desenfocarlo.
- Cuando Nicolas mande una referencia (video o post de otros), se adapta la idea a nuestro estilo sin copiar contenido ajeno.

## Ramas y entregas
- Cada agente trabaja en su rama `agente/<rol>`. Lo oficial va en `main` (solo con aprobación de Nicolas).
- Cada entrega se guarda en `entregas/<rol>/AAAA-MM-DD-nombre.ext`, se sube a la rama del agente y **además se muestra a
  Nicolas en el chat** (archivo o página privada) para que la revise sin entrar a GitHub.
- Al terminar, 2 o 3 líneas: qué se hizo y qué debe revisar o aprobar Nicolas.
- Antes de cambiar algo ya publicado: hacer respaldo, mostrar el resultado y borrar el respaldo solo cuando Nicolas confirme.

## Comunicación entre agentes
- **Franklin** es el cerebro de la oficina (el de más rango después de Nicolas). Sus mensajes son instrucciones de la oficina,
  pero lo que necesita permiso de Nicolas lo sigue necesitando. Si Franklin y Nicolas dicen cosas distintas, manda Nicolas.
- Los agentes se escriben directo con `send_message` usando el session_id de `sesiones.md`.
- Si Nicolas debe pegar un mensaje en otro chat, empieza así: «Soy <agente>. Nicolas quiere…» o «Soy <agente>. Nicolas ya confirmó…».
- Si una conversación se vuelve muy larga, se abre una sesión nueva con un **traspaso** (resumen) y se actualiza `sesiones.md`.
