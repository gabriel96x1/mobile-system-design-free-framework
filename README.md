# Como abordar entrevistas de systems design para Mobile Devs (WIP)
A countinuación vamos a mostrar una forma sencilla para enfrentar entrevistas de "Systems Design" Mobile Devs. Es importante tener en cuenta que la solución que propongas no tiene que ser perfecta, ya que el propósito de esta etapa no es crear un sistema completo en 30 minutos. En realidad, lo que el entrevistador valora son las "señales" que reflejen cómo piensas, cómo te comunicas y cómo abordas problemas complejos. Cada idea que compartas y cada decisión que tomes deben destacar tus habilidades y brindar al entrevistador una visión clara de tu potencial como candidato.

# Proceso de entrevista convencional (45 – 60 min)
- 2 – 5 min - presentaciones
- 5 min - definición del alcance y toma de requerimientos
- 10 min - discusión de detalles a alto nivel
- 20 - 30 min - discusión de detalles de implementación
- 5 min - preguntas para el entrevistador

# Presentaciones
Usualmente el entrevistador te dirá que le cuentes o le platiques acerca de ti, para esto suele ser recomendable tener preparado un "Elevator Pitch" de 2 min aproximadamente, en el cual expliques de forma consistente cual ha sido tu experiencia laboral, y que partes de tu conocimiento te hacen un candidato ideal, en ocaciones es bueno agregar el por que te gustaría trabajar para la compañia a la que estás aplicando.

# 1 - Define el alcance de lo que vas a trabajar
El entrevistador es quien plantea la tarea. Por lo que te pedirá de realices el diseño de un sistema o aplicación móvil con ciertas características que no siempre son del todo claras. Lo primero que debes hacer es entender el alcance del lo que vas a abordar:

- *Solo la parte del cliente:* en este caso, solo te enfocarías en la aplicación móvil, dando por hecho que el backend y la API ya están desarrollados y disponibles.

- *Cliente + API:* este es el escenario más frecuente en las entrevistas. Aquí tendrías que diseñar tanto la aplicación móvil como la API que estaría consumiendo la aplicación.

- *Cliente + API + Backend:* es menos convencional que suceda, ya que muchos ingenieros de apps móviles no tienen experiencia directa en el backend. Si te preguntan sobre temas relacionados con el servidor, lo mejor es ser transparente y admitir que tu expertise está más enfocado en el lado del cliente y que no tienes experiencia práctica en el backend. Siempre es mejor ser honesto que intentar aparentar conocimientos que no tienes. Si el entrevistador insiste, puedes explicar que lo que sabes sobre backend proviene de recursos como libros, videos en YouTube o blogs especializados, pero no experiencia propia por lo que tus recursos serán más limitados.

# 2 - Toma de Requerimientos
Puedes dividir la toma de requerimientos en: Funcionales, No funcionales, Fuera del alcance y Dominio o Requerimientos de Negocio

## Requerimientos Funcionales
Toma de 3 a 5 requerimientos que sean funcionalidades escenciales para el problema propuesto.
Ejemplos:
- El usuario necesita poder escrollear en una lista infinita.
- El usuario necesita poder crear una nueva publicación.
- El usuario necesita poder cambiar su foto de perfil.

## Requerimientos No Funcionales
Son funcionalidades no visibles para el usuario pero de suma importancia para una buena experiencia.
Ejemplos:
- La aplicación debe de ser offline/online first.
- La aplicación debe soportar notificaciones en tiempo real.
- La aplicación guardará datos sensibles encriptados en local.
- La aplicación debe de implementar un sistema de caching para imagenes.
- La aplicación debe implementar un sistema que prevenga llamadas constantes a una api.

## Fuera de alcance
Son las funcionalidades que no se tocarán a la hora de hacer el diseño de la arquitectura.

## Dominio o Requerimientos de Negocio
Son requerimientos necesarios para cumplir con regulaciones de ciertas industrias.
Ejemplos:
- Salud: El software debe cumplir con las regulaciones HIPAA para el manejo de datos de pacientes.
- Finanzas: El sistema debe adherirse a los estándares GAAP para la elaboración de informes financieros.
- Comercio electrónico: El software debe ser compatible con diversas pasarelas de pago, como PayPal, Stripe y tarjetas de crédito.

### Lo que busca el entrevistador 👀
Las preguntas de diseño de sistemas suelen ser ambiguas. El entrevistador está más interesado en observar tu proceso de pensamiento que en la solución concreta que propongas:
- ¿Qué cosas asumiste y cómo lo planteaste?
- ¿Qué características elegiste incluir?
- ¿Qué preguntas aclaratorias hiciste?
- ¿Qué preocupaciones y trade-offs mencionaste?

# 3 - Preguntas de composición de tu equipo
- ¿Cuántos ingenieros integrarán el equipo?
Construir un producto con un equipo pequeño (de 2 a 4 ingenieros): La principal preocupación será la simplicidad, no hay estricta necesidad de modularización y el trabajo de features vistas como MVPs

Construir un producto con un equipo grande (de 20 a 100 ingenieros): La principal preocupación es la estructura del proyecto y su modularización. Debes diseñar tu sistema de manera que permita que varias personas trabajen en él sin interferir en el trabajo de los demás.

