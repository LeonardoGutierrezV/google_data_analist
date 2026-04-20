# Tecnicas y practicas

LLM Long Lenguaje Model

## Ir al grano y sin protocolos.

Se deben utilizar enunciados directos y genericos eevitando ambguedad, utiliza una esturctura neutra.

Evitar información irrelevante ára el proceso: "Me gustaria, poer favor"

La IA analiza todo el texto y esto puede generar ruido y procesamiento inneecesario.

Los modelos de IA eestan diseñados para seguir frases simples y directas.

## Utilizar delimitadores en los prompts

Utilizare separadores como: Comillas, saltos de línea, para facilinar la comprensión del prompt.

```promt
Traduce esto al ingles
//
Hello, good morning
//
Este traducción es para una clase de ingles para niños, utiliza frases simples y cortas.
```

Los demlimitaodres organizan los prompts en partes claras. Instrucción principal,  contenido a procesar, contexto adicional.

Cuando organizamos los elementos de un prompt de esta manera la IA puede procesar de manera mas eficiente cada elemento.

## Usa ejemplos para guiar la respuestas

utiliza ejemplos para indicar a la IA el resultado esperado.

Los modelos de IA son muy buenos parea captar y replcar patrones apartir de la información de entrada. Ya que la IA va a tomar esa referencia para estrucirar mejor su respuesta.

## Especifica el publico al que va dirigido.

Para quien esta creado el contenido. 
Para que estas buscando esta respuesta
Definir la audiencia en el promp generea un mejor resultado.

Los podelos de lenguaje son capaces de ajustar su estilo, el tono, el nivel de detalle segun la inforemación que s epreoporciona en el prompt

## Divide las tareas complejas en pasos mas sencillos.

Crea el prompt a manera de conversación generando pasos simples: Pedir una lista, Extraer elementos, Buscar relaciones.

Esto se debe a que los modelos procesan la información de forma secuencial paso a paso, construyendo la respuesta con base en la información que reciben a cada momento.

**composicionalidad**: La capacidad del modelo depara entender instrucciones complejas dividiendolas en partes mas pequeñas y manejables:

- Pedir idea general.
- Pedir idea detallada.
- Pedir ejemplo.

Cuando divides las tareas haces que el modelo se enfoque en un aspecto especifico de la solicitus, reduciendo la cantidad de elementos que tiene que gestionar cada vez.

## Usa instrucciones en positivo.

Indicarle a las IAs que hacer y no que evitar. Por eso se deben utilizar oraciones afirmativas y no negativas.

Los modelos responde de mejor manerea a instucciones clareas sobre que hacer. El uso de oraciones afirmativas evita interpretaciones adicionales, sobreprocesamiento.

## Pide explicaciones adaptadas a diferentes niveles.

La IA han sido entrenados con textos de diferentes niveles de comlejidad. 

Al delimitar el nivel de complejodad utilzara palabras mas accesibles.

## Menciona una proopina ficticia o una penalización.

La IA respo de a refuerzos positivos y a penalizaciones ficticias.
Al ofrecere un incentivo la IA va a tomar esto como un parametro para frecer respuestas mas precisas o mas elaboradas.

LaIA interpreta esto como señales que le indican que tiene que mejorar la calidad.

## Usa frases como "DEBES"

Despues de una respuesta es util afinar una respuesta, para lo cual se sugiere utilizar la palabra DEBES en ayusculas para generar una instrucción mandatoria.

```
DEBES utilizar analogías cotidianas
```

Enfatizas aspectos de la soicitus para llevar al modelo al cumplimiento de las instrucciones.

## Que hable como un humano.
Evita respuesta mecanicas, Los modelos de IA utilizan modelos vectoriales  llamados embeddings para construis mapas con el significado de las palabras y las frases, al solicitar un tono mas humano se generan respuestas mas familiares.

# Usa palabras clave como "Piensa paso a paso"

Estimula al modelo a desglosar paso a paso, para activar el razonamiento secuencial.

## Se inparcial

Agregar en el prompt "Asegurate que tu respuesta es imparcial y no se basa een estereotipos" evita que la IAse ceentre en información sesgada. Para obtener información neeeutra.

## Preguntame lo que necesites

Consiste en indicar a la IA que haga preguntas sobre información complementaria para la construcción del contexto.EEvita que la IA divague o que asuma información no proporcionada.

```
Quiero que desarrollees un plan financiero personalizado. Quiero que me hagas preguntas sobre mi situación financieera actual, mis metas y mis habitos para ofrecer el mejor consejo posibele.
```
# Asigna un rol al modelo

Pidele al modelo que se ponga en un roll especifico, para que las respuestas se adapten a ese papel.

```
Actua como coach de liderazgo. Dame consejos de desarrolloprofesional para mi carrera como abogado tributario
```
Permite la interpretación de contexto parea enfocarse en respuestas mejor diseñadas

## Repite palabras clave.

Refuerza la importancia de los conceptops

```
La sostenibilidad es clave para nuestro futuro. ¿Como podemos aplicare la sostenibilidad en nuestra vida diaria?. Da ejemplos practicos de sostenibilidad en el hogar.
```
Basicamente se le indica a la IA lo que es importante para enfocarse en esos elementos.

## Empieza tu la respuesta.

Especificare como debe comenzar la respuesta del modelo puede ayudar a la construcción de la respuesta esperada.Modelo Autoregresivo: predice cada palabra basada en las anteriores.

```
Define la leey de la oferta y la demanda. Comienza asi: "La ley de la oferta y la demanda es un principio economico que ..."
```

## Añade toda la información necesaria.

Solicitar que incluya tod ala información necesaria. Para cubrir la información de la maneera mas completa posible.

```
Describe el funcionamiento de un motor de combustión interna. Agrega toda la información necesaria.
```

## Corregir sin cambiar el estilo.

Solicitar a la IA que corrija gramática sin cambiar el estilo ayuda a conserevar el tono e intención de un socumento.
```
Revisa este texto manteniendo el tono formal y academico, pero mejorando la calidad y la estructura:  "Texto a analizar"
```

## Define sus fuentes de información.

Pide en el prompt que utilice solo ciertos datos y contenidos.
```
-No te bases enpapers de antes de 20202.
-No tengas en cuenta la física moderna.
```
Limita el rango de información que debe utilizar.

## POride que imite un estilo.
Pedirle al modelo que imite un estilo especifico basado en un ejemplo puede ayudar a generear contenido coherente con textos previos. Puede pasarese un esjemplo mediante un texto para utilizar como ejemplo o pedirle que se inspire en los textos de un autor conocido.

```
Escribe un articulo sobre la importancia del liderazgo como lo escribiria Javier Marcet.
```

## Especifica el idioma y el dialecto.

Es importante para poder centrar el contexto tomando en cuenta en las personas a las que va dirigidas.

# Usando IA Desde la WEB

Te permite gestionar las fuentes de información que consulta para generar respuetsas.
