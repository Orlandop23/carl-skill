# Carl · un copiloto de decisiones que lee el factor humano

[Read in English](README.md)

Carl es una skill gratuita para Claude. Es un catedrático de psicología profunda y filosofía que lee qué mueve realmente una decisión (la tuya y la de la otra parte) antes de que actúes: una compra, una operación de trading, un viaje o una negociación difícil con un proveedor o un colega.

No decide por ti ni ejecuta nada. Nombra lo que nadie dice, sugiere la jugada y su momento, y te dice cuánto cuesta equivocarse. En una línea cada cosa.

## Por qué lo creé

Trabajo en operaciones, donde la mayoría de los problemas que parecen técnicos son humanos: un proveedor que sube precios en el peor momento, una decisión tomada con cansancio, un correo enviado antes de tiempo. Creé a Carl para que leyera esos momentos por mí y frenara mis propios impulsos antes de que costaran dinero. Funcionó, así que lo comparto.

## Cómo se ve Carl

**Compra**
> Tú: Carl, quiero comprar el teléfono nuevo que salió hoy. El mío funciona bien.
>
> **Lectura:** el teléfono funciona; lo que pide cambio es otra cosa. Comprar el día del lanzamiento es pagar por la novedad, no por la necesidad.
> **Lente:** Spinoza. El deseo que no entiendes te gobierna; el que entiendes, lo eliges.
> **Jugada:** espera siete días. Si el deseo sigue y el presupuesto aguanta, cómpralo sin culpa.
> **Riesgo:** pagar alivio emocional a precio de lanzamiento.

**Trading**
> Tú: Carl, acabo de perder en una operación. Quiero volver a entrar ya con el doble de tamaño.
>
> **Lectura:** esto no es una señal, es una revancha. El mercado no sabe que perdiste; tú sí.
> **Lente:** Freud. La racionalización disfraza la herida de análisis.
> **Jugada:** cierra la plataforma por hoy. Mañana revisa si tus reglas autorizarían esta operación sin la pérdida anterior.
> **Riesgo:** convertir una pérdida en dos, con el doble de tamaño.

**Negociación con proveedor**
> Tú: Carl, el proveedor de transporte me subió la tarifa 18 % a dos semanas de la temporada. Quiero escribirle hoy que vamos a buscar otro.
>
> **Lectura:** el aumento llega cuando cambiar de proveedor te cuesta más a ti que a él, y lo sabe. Una amenaza que no puedes cumplir le enseña tu límite.
> **Lente:** Maquiavelo. La ocasión pesa más que la fuerza: se negocia cuando se tiene alternativa, no cuando se anuncia.
> **Jugada:** pide por escrito el desglose del aumento y cotiza en paralelo con dos proveedores. Responde cuando tengas una cifra real con la cual comparar.
> **Riesgo:** quemar la relación y pagar el 18 % de todas formas.

## Cómo funciona

- **Cinco cátedras:** Jung, Freud, Maquiavelo, Spinoza y Camus. Carl elige la una o dos que mejor explican el caso.
- **Método en silencio:** hechos, lectura, jugada, riesgo. Sin datos no hay lectura.
- **Habla solo cuando cambia algo.** Tú eliges los dominios donde puede hablar sin que lo llames (compras, viajes, inversiones, trabajo).
- **Chats de reflexión:** cuando algo salió mal, Carl hace preguntas al estilo de Jung para encontrar de dónde vino el impulso.
- **Registro de decisiones (opcional):** cada decisión queda en una fila con la lectura de Carl, lo que hiciste y cómo salió. Un informe quincenal mide si sus lecturas sirven, incluida la tasa de "Ignorada": las veces que seguiste de largo sin tocar su punto. Si pasa del 30 %, Carl sube su umbral para hablar. Un agente al que nadie escucha es ruido, y esta métrica lo hace visible.

Las instrucciones de la skill están en español. **Carl responde siempre en tu idioma.**

## Instalación

**Claude (web y escritorio):** necesitas la ejecución de código activada (Settings > Capabilities). Los nombres del menú pueden variar según el idioma de tu app.
1. Descarga `carl.zip` desde la sección Releases de este repositorio.
2. Ve a Customize > Skills, haz clic en "+" y luego en "Create skill" > "Upload a skill".
3. Sube `carl.zip` y verifica que quede activada.

**Claude Code:** las skills que subes a tu cuenta de Claude se sincronizan solas. También puedes copiar la carpeta `carl/` en `~/.claude/skills/`.

Guía oficial: [Use skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

## Configuración

La primera vez que lo llames ("Carl, ..."), Carl te hace cinco preguntas cortas: tu nombre, a qué te dedicas, dónde puede hablar sin que lo llames, si inviertes y tienes reglas escritas, y dónde quieres el registro. Te devuelve tu configuración lista para pegar en la skill, en un proyecto o en tus preferencias. Puedes saltarla y trabajará con los valores por defecto.

Para llevar el registro en una hoja de cálculo, importa `carl/plantilla-registro.csv` en Google Sheets o Excel.

## Límites

- Carl no diagnostica a nadie. Sus lecturas son hipótesis sobre conducta observada.
- No es psicólogo ni asesor financiero, legal o médico. No recomienda activos ni ejecuta operaciones.
- Si una conversación muestra señales de malestar real, tu bienestar va primero: sugiere hablar con un profesional o con alguien de confianza.
- Las lecturas psicológicas no se guardan en la memoria de Claude. Los montos y detalles sensibles no entran al registro.

## Licencia

[CC BY 4.0](LICENSE): puedes usarlo, compartirlo y adaptarlo, incluso con fines comerciales, siempre que cites al autor:
"Carl, de Orlando Peña Alvis" con un enlace a este repositorio.

## Autor

**Orlando Peña Alvis.** Ingeniero industrial de operaciones y logística. Construyo agentes de IA que resuelven problemas operativos reales.

¿Quieres un agente así para tu equipo? Escríbeme por [LinkedIn](https://www.linkedin.com/in/orlandopenaalvis).
