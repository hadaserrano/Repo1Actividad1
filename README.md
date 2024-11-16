# AD-1 Tarea en equipo. Control de versiones con GIT

## Repositorio

https://github.com/hadaserrano/Repo1Actividad1

## Integrantes

* Hada Sánchez Serrano [@hadaserrano](https://github.com/hadaserrano)
* Andrés Budziszewski González [@AndresBudziszewski](https://github.com/AndresBudziszewski)
* Jesús Castañer Moreno [@jesuscastaner](https://github.com/jesuscastaner)
* Ramón Alarcón Fernández [@Ramon-unir](https://github.com/Ramon-unir)
* Cristian Osso Parra [@cristian0612](https://github.com/cristian0612)
* Mireia Boldú Valldeoriola [@MiaBV](https://github.com/MiaBV)
	
## Requerimiento 1

Para comenzar, Hada creó un nuevo repositorio en GitHub e incorporó a los demás compañeros como colaboradores. Este repositorio sólo contenía entonces un archivo README.md.

A continuación, Jesús clonó el repositorio creado por Hada en su máquina y generó la estructura de carpetas y archivos del enunciado, utilizando los comandos `mkdir` para los directorios y `touch` para los archivos. También configuró el archivo .gitignore añadiendo en su interior los elementos que debían ignorarse:

* gitignore
* archivos_privados
* *.psd
* *.xcf

También en este punto Jesús creó su archivo HTML personalizado, lo añadió todo al stage con `git add`, hizo `commit`, hizo `merge` de su rama develop a su rama _main_, y finalmente actualizó el repositorio remoto con `git push`.

Sin embargo, al reunirnos posteriormente para trabajar en conjunto decidimos eliminar todos los elementos del repositorio compartido (todas las carpetas y archivos) y reconstruirlos de nuevo para que todos los colaboradores pudiéramos observar y practicar cómo hacerlo desde el principio. Nótese que en esta nueva ocasión nos olvidamos de crear el archivo index.html, que fue añadido por Cristian más adelante, antes de comenzar el Requerimiento 3.

Cada colaborador clonó localmente el repositorio remoto utilizando `git clone` y creó su propio archivo HTML personalizado en una rama _develop_ particular, que cada uno denominó con su propio nombre (ramas _jesus_, _hada_, _andres_, _cristian_, _mia_ y _ramon_). Luego, cada colaborador añadió su archivo HTML al stage, realizó el `commit`, hizo un `merge` de su rama _develop_ a la rama _main_, y terminó con un `push` al repositorio remoto.

Este requerimiento fue el que más nos costó debido a que no estábamos aún muy familiarizados con Git/GitBash, ni con la estructura interna del repositorio. Como se puede observar en el historial de commits del proyecto, los primeros pasos fueron muy tediosos y desorganizados. Tanto en este requerimiento como en los siguientes, los integrantes del grupo han trabajado individualmente pero uniendo sus esfuerzos en dos sesiones sincrónicas de Discord, que han superado las 10 horas de duración. En ambas sesiones nos hemos comunicado en inglés para facilitar la inclusión y colaboración de uno de los integrantes cuyo idioma nativo es ése.

# Requerimiento 2 

Este paso lo fuimos haciendo de uno en uno, esperando todos a que un colaborador terminara y subiera su trabajo antes de comenzar con el siguiente. Con la idea de generar conflictos de forma intencionada, se nos ocurrió que, por parejas, se harían modificaciones en el archivo index.html, pero partiendo de que uno de ellos estuviese un commit por detrás para que, al intentar realizar un merge con su rama _main_, le generase un "conflict" que ambos tendrían que resolver poniéndose de acuerdo sobre qué versión escoger para solucionarlo.

Cada participante actualizó su repositorio local con `git pull`, y a continuación añadió una lista de 3 hobbies a su archivo HTML. Una vez hecho, añadió su archivo modificado al stage, hizo `commit`, hizo `merge` de su rama _develop_ a la rama _main_ y, por último, hizo `push` para actualizar el repositorio remoto.

En cada paso se fue haciendo `git status` para verificar cuidadosamente el estado del repositorio. Los demás colaboradores comprobamos después de cada `push` que los cambios se reflejaran correctamente en GitHub, y a continuación otro de nosotros hacía `pull` y repetía el proceso hasta terminar todos.

Al final de este requerimiento, se hizo `commit` y `push` por error de la eliminación del archivo README.md, que sería reañadido por Jesús al repositorio compartido al final de la actividad.

Nótese que Ramón no completó su parte de este requerimiento hasta más adelante debido a problemas técnicos con su equipo.

# Requerimiento 3

En primer lugar, Cristian y Mireia actualizaron sus repositorios locales con `git pull` y ambos realizaron pequeños cambios en una misma línea del archivo index.html desde sus respectivas ramas _develop_. Ambos realizaron un `commit` de sus modificaciones, pero sólo Cristian fusionó su rama _cristian_ con la rama _main_ y subió los cambios al repositorio remoto con `git push`. Nuevamente, se verificó el estado del repositorio con `git status` a cada paso.

A continuación, Mireia hizo `pull` en su rama _main_ y trató de hacer `merge` de su rama _mia_ a su rama _main_, como había hecho Cristian, obteniendo un conflicto. Mireia lo resolvió decidiendo quedarse con su propia versión, de modo que, cuando hizo `push`, la versión de Cristian quedó sobreescrita en el repositorio remoto.

Repitieron el proceso algunas veces más Jesús, Andrés, Hada y Ramón.

Si bien este requerimiento era, al menos en su planteamiento, algo más complejo que los anteriores, donde nos encontramos con bastantes problemas, nos resultó una experiencia mucho más sencilla y fluida, como puede observarse de comparar la última parte del historial de commits con la inicial. En este punto todos estábamos mucho más familiarizados con los comandos básicos de Git y con el manejo de la terminal en general, y la práctica de trabajar juntos en entender y resolver los problemas de las fases anteriores contribuyó a que termináramos interiorizando la estructura general de todo lo que es el proceso del trabajo colaborativo en un repositorio compartido. En términos generales, la conclusión es que ha habido un proceso creciente de aprendizaje que consideramos muy positivo. 

Al finalizar, Ramón realizó el Requerimiento 2 que había quedado pendiente, añadiendo los 3 hobbies a su archivo HTML.

Por último, Jesús añadió el contenido de este documento a un README.md y lo subió al repositorio remoto.