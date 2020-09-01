# Producto_Unidad2
# Informe 
##  Implementación de una interfaz HMI en NODE-RED  y el Diseño de una calculadora científica en Python

## 1.PLANTEAMIENTO DEL PROBLEMA

Conocer  los diferentes nodos que nos ofrece la plataforma NODE-RED para poder implementarlos en una Interfaz Humano Máquina. Analizar los pines de la Raspberry Pi para poder usarlos en el programa de una calculadora científica por medio del lenguaje de programación Python



## 2.OBJETIVOS

### General:

Identificar las características de los nodos capaces de poder utilizarlos en una una interfaz HMI y las propiedades de los pines de la GPIO que nos ofrece la Raspberry Pi.

### Específicos:

> Explorar las bibliotecas de notas y de funciones que nos ofrecen NODE-RED y Python respectivamente.
 
> Comprender la sintaxis y la semántica de la programación orientada a objetos de Python.




## 3.ESTADO DEL ARTE

### Tema: Adquisición de datos desde plataforma IOT2040. Protocolos MODBUS/TCP y OPC UA

Investigadores: Calvo Luis, Borja.

Año: 2019

Este trabajo se basa en la adquisición de datos de un proceso automatizados desde dispositivo SIMATIC IOT2040 de SIEMENS, con diferentes protocolos industriales, mediante una plataforma de programación (Node-RED). Así, se posibilita la lectura, envió y procesamiento de datos de un proceso en un servidor remoto, facilitando la implementación de la industria 4.0 a través del Internet de las Cosas (IoT) a cualquier proceso automatizado futuro.
 
Lan hau automatizazio prozesu datuen eskuratzean oinarritzen da SIMATIC IOT2040 gailuaren bidez, protokolo industrial desberdinekin, programazio plataforma baten (Node-RED) bitartez. Horrela, prozesuko datuen irakurketa, bidalketa eta prozesaketa zerbitzari urrun batean posible egiten da, 4.0 industriaren inplementazioa erraztuz Gauzen Internetaren (IoT) bidez etorkizuneko edozein automatizazio prozesutarako.


Lugar: Universidad del País Vasco / Euskal Herriko Unibertsitatea.


### Tema: Programación de una librería de Python capaz de leer ficheros PDB para representar proteínas en 3D.

Investigadores: Cabrelles Muñoz.

Año:2018

Este proyecto tiene como finalidad el uso de librerías de Python para la visualización de estructuras proteicas tridimensionales mediante el procesado de archivos PDB. Para ello, se utilizaron las herramientas ofrecidas por BioPython para el procesado de datos, y las librerías matplotlib y VisPy para la visualización de los datos procesados. El resultado de este trabajo es un programa cuya interfaz gráfica fue creada mediante la librería Tkinter, que permite la selección del archivo a representar, la selección del motor que se utilizará para la visualización y qué tipo de visualización se generará (CPK, según el tipo de aminoácido al que pertenece, dividido en cadenas, y usando DSSP).

Lugar: Universitat Oberta de Catalunya, España.
 
## 4.MARCO TEÓRICO


 
### Node-RED
 
Node-RED es una herramienta de programación para conectar dispositivos de hardware, API y servicios en línea de formas nuevas e interesantes.
 
Proporciona un editor basado en navegador que facilita la conexión de flujos utilizando la amplia gama de nodos en la paleta que se pueden implementar en su tiempo de ejecución con un solo clic.
 
![](IMG/node.png)

### Características de Node-RED
 
Node-RED proporciona un editor de flujo basado en navegador que facilita la conexión de flujos utilizando la amplia gama de nodos en la paleta. Los flujos se pueden implementar en tiempo de ejecución con un solo clic.
 
Las funciones de JavaScript se pueden crear dentro del editor utilizando un editor de texto enriquecido.
 
Una biblioteca incorporada le permite guardar funciones, plantillas o flujos útiles para su reutilización.
 
El tiempo de ejecución ligero se basa en Node.js, aprovechando al máximo su modelo sin bloqueo controlado por eventos. Esto lo hace ideal para ejecutarse en el borde de la red en hardware de bajo costo, como Raspberry Pi, así como en la nube.
 
Con más de 225,000 módulos en el repositorio de paquetes de Node, es fácil extender el rango de nodos de paleta para agregar nuevas capacidades.
 
### Comunidad  de Node-RED
 
Los flujos creados en Node-RED se almacenan utilizando JSON, que se puede importar y exportar fácilmente para compartir con otros.
 
Una biblioteca de flujo en línea le permite compartir sus mejores flujos con el mundo.

### Nodos
 
Node RED al ser una herramienta de programación visual nos despliega una barra donde podemos encontrar diversos tipos de nodos, los cuales podemos conectarlos para poder hacer nuestro programa, recalcando que cada nodo cumple una función en específico. Entre estos están los nodos:


> Audio out : 

Un widget que le permitirá reproducir audio (wav o mp3) o enviar texto a voz (TTS) al cliente.

> Button : 

El ícono se puede configurar usando los íconos Material o fa; también se puede configurar el color y el color de fondo. Si el widget tiene un tamaño de 1 ancho, el icono tiene prioridad.

> Chart  : 

Tiene modos de línea, barra y gráfico circular. Además, las etiquetas del eje X se pueden personalizar utilizando una cadena de formateador de fecha. Consulte este documento para obtener más información sobre los formatos de datos de gráficos aceptados.

> Colour Picker : 

Un widget de selector de color.

> Date Picker : 

Un widget de selector de fecha. El formato de fecha mostrado se puede especificar en la pestaña Sitio usando el formato moment.js.

> Dropdown : 

Se ha agregado un widget de selección desplegable. Etiqueta múltiple, se pueden especificar pares de valores. Las opciones también se pueden establecer a través de msg.options que contienen una matriz de objetos.

> Form : 

Un widget que puede estar compuesto por varios sub-widgets. Cuando se envían, todos los valores se envían como un solo mensaje.

> Gauge : 

Tiene 4 modos: estándar (indicador simple), donut (360 ° completo), brújula y onda. También puede especificar la gama de colores de los medidores estándar y de rosquilla.

> Notification : 

Crea alertas al usuario, puede ser una ventana emergente de brindis o un cuadro de alerta descartable. La alerta puede estar dirigida a un solo usuario.

> Numeric : 

Un widget de entrada numérico con botones arriba / abajo.

> Slider : 

Un control deslizante horizontal simple, con un tamaño de paso variable.

> Switch : 

Interruptor: también puede establecer dos iconos y / o colores según el estado.

> Template : 

El nodo de plantilla permite al usuario especificar y crear sus propios widgets dentro del marco utilizando HTML, Javascript. Este es un widget Angular.js. También puede usar esto para anular los estilos CSS incorporados.

> Text : 

Se puede configurar un widget de solo lectura, el diseño de la etiqueta y el valor.

> Text input :

El cuadro de ingreso de texto, con etiqueta opcional, también puede admitir modos de contraseña, correo electrónico y color.

UI-Control: 

Permite un control dinámico del tablero de instrumentos. Enviar un msg.payload del número de pestaña a otro, para cambiar a esa pestaña. Las pestañas se pueden habilitar, deshabilitar, ocultar, mostrar mediante mensaje.Esto se puede usar para activar otras acciones, como restablecer la visibilidad de pestañas y grupos.

![](IMG/22.PNG)
 
### Python
 
Python fue creado a finales de los ochenta por Guido van Rossum en el Centro para las Matemáticas y la Informática (CWI, Centrum Wiskunde & Informatica), en los Países Bajos, como un sucesor del lenguaje de programación ABC, capaz de manejar excepciones e interactuar con el sistema operativo Amoeba. El nombre del lenguaje proviene de la afición de un grupo británico de comediantes conocidos como Monty Python. (Python, n.d.)
Python es un lenguaje de programación interpretado el cual hace hincapié en la legibilidad de su código. Se trata de un lenguaje de programación multiparadigma, ya que soporta orientación a objetos, programación imperativa y, en menor medida, programación funcional.
Este lenguaje está administrado por la Python Software Foundation. es una organización sin fines de lucro creada el 6 de marzo de 2001 dedicada al lenguaje de programación Python. Es responsable de varios procesos dentro de la comunidad, como el desarrollo de Python, la administración de los derechos intelectuales y de obtener fondos.(Operadores Python ➞ Explicamos Todos Los Operadores + Ejemplos Reales, n.d.)
 
![](IMG/2-25.jpg)
 
Los pasos para comenzar con Python en la programación de una interfaz de usuario no son terriblemente complejos, pero requiere que el usuario empiece a tomar algunas decisiones. Por su naturaleza como un lenguaje de programación de propósito general con intérpretes disponibles en todos los sistemas operativos comunes, Python tiene que ser bastante agnóstico en cuanto a las opciones que presenta para crear interfaces gráficas de usuario.
Afortunadamente, hay muchas opciones disponibles para los programadores que buscan crear una manera fácil para que los usuarios interactúen con sus programas. Existen enlaces para varios frameworks de interfaz de usuario en una variedad de plataformas, incluidas las nativas Windows, Mac y Linux, y muchas que funcionan en las tres.
En este punto, tiene que evaluar bien el hecho de necesitar una interfaz gráfica. Al momento de desarrollar una aplicación, también debe considerar una interfaz web, especialmente si cree que los usuarios puedan querer alojar su aplicación de forma remota, y proyectos como Django, Flask o Pyramid hacen que esto sea sencillo. Incluso puede usar una librería como pywebview para colocar una capa delgada alrededor de una aplicación web en una ventana GUI más nativa.
 
 
 
### RASPBERRY PI
 
Raspberry PI es una placa computadora (SBC) o Pc de placa única, de bajo precio, se podría expresar que es un ordenador de tamaño reducido, del orden de una tarjeta de crédito, desarrollado en el Reino Unido por la Fundación Raspberry PI (Universidad de Cambridge) en 2011, con el objetivo de estimular la enseñanza de la informática en las escuelas, aunque no empezó su comercialización hasta el año 2012. El concepto es el de un ordenador desnudo de todos los accesorios que se pueden eliminar sin que afecte al funcionamiento básico. Está formada por una placa que soporta varios componentes necesarios en un ordenador común y es capaz de comportarse como tal. A la Raspberry Pi la han definido como una maravilla en miniatura, que guarda en su interior un importante poder de cómputo en un tamaño muy reducido. Es capaz de realizar cosas extraordinarias(Yamanoor, Narasimha Saii,Yamanoor, 2013)
 
Los componentes de la Raspberry Pi son:
 
●	Un Chipset Broadcom BCM2835, que contiene un procesador central (CPU) ARM1176JZF-S a 700 MHz (el firmware incluye unos modos Turbo para que el usuario pueda hacerle overclock de hasta 1 GHz sin perder la garantía)
 
●	Un procesador gráfico (GPU) VideoCore IV
 
●	Un módulo de 512 MB de memoria RAM (aunque originalmente al ser lanzado eran 256 MB).
 
●	Un conector de RJ45 conectado a un integrado lan9512 -jzx de SMSC que nos proporciona conectividad a 10/100 Mbps
 
●	2 buses USB 2.0
 
●	Una salida analógica de audio estéreo por Jack de 3.5 mm.
 
●	Salida digital de video + audio HDMI
 
●	Salida analógica de video RCA
 
●	Pines de entrada y salida de propósito general
 
●	Conector de alimentación microUSB
 
●	Lector de tarjetas SD
 
(Yamanoor, Narasimha Saii,Yamanoor, 2013)
 
### Puerto GPIO de la  RASPBERRY PI
 
La placa Raspberry Pi puede comunicarse con dispositivos externos a través del conector GPIO incorporado. En este conector hay pines de alimentación integrados (+5 y +3.3 V), tierra y pines de entrada / salida capaces de implementar diferentes protocolos.
 
Dado que existen dos versiones diferentes de hardware Raspberry Pi (rev. 1 y 2), las asignaciones de puertos también pueden variar. Sin entrar, en este momento, en los detalles de los protocolos, las dos posibles versiones de nuestra Raspberry Pi nos llevan a dos posibles escenarios de hardware. Podemos ver aquí un pin de diagrama comparativo de numeración GPIO.
 
#### Los pines GPIO tienen funciones específicas:
 
El color amarillo (2): Alimentación a 3.3V.
 
El color  rojo (2): Alimentación a 5V.
 
El color naranja (26): Pueden configurarse como entradas o salidas se las conoce también como pines de Propósito General.
 
El color gris (2): Son pines reservados.
 
El color negro (8): Conexión a GND.
 
El color azul (2): Comunicación mediante el protocolo I2C (Circuito inter-integrado).
 
El color verde (2): Destinados a conexión para UART para puerto serie convencional.
 
El color morado (5): Comunicación mediante el protocolo SPI (Es un protocolo síncrono, el cual sincroniza y transmite datos  por medio de 4 señales).
 
 ![](IMG/esquema-pines-gpio.png)


### Create.withcode.uk online
 
Create.withcode.uk es un editor de python en línea que le permite escribir, ejecutar, depurar y compartir código de python en su navegador web. Se lanzó en abril de 2016 para ayudar a los estudiantes a aprender a escribir código en cualquier dispositivo sin tener que instalar ningún software especializado.

Todos los recursos en este sitio se publican bajo la licencia Creative Commons de uso compartido, lo que significa que puede usar cualquier cosa aquí para cualquier propósito, siempre y cuando me haga referencia como autor original. Sin embargo, hasta ahora, aunque create.withcode.uk ha sido de uso gratuito, el código fuente que lo hace funcionar no ha estado disponible de forma abierta.

Create.withcode.uk ahora es de código abierto. Esto significa que si puede pensar en una forma de mejorar el editor de Python o detecta un error que necesita reparación, no tiene que esperar a que lo codifique: puede saltar y adaptarlo / ampliarlo / mejorarlo te gusta. Puedes usarlo libremente para tus propios proyectos.

#### Prestaciones

> Autoevaluación de pruebas de python que se integran con moodle

> Crea juegos y objetos en 3D usando python

> Cuestionarios interactivos de python que se integran con moodle


![](IMG/2.PNG)

## 5. DIAGRAMAS

![](IMG/pi_board_pinout.jpg)

## 6. LISTA DE COMPONENTES 

#### Diseño una calculadora científica en Python

- Interner
- Plataforma create.withcode.uk online
- Computador
- Python

#### Implementación de una interfaz HMI en NODE-RED

- Internet
- NODE.JS
- Plataforma NODE-RED
- Computador
 
## 7. MAPA DE VARIABLES

#### Diseño una calculadora científica en Python

![](IMG/MAPAvARIABLEcALCULADORA.JPG)

#### Implementación de una interfaz HMI en NODE-RED

![](IMG/nod.PNG)


## 8. APORTACIONES

#### Diseño una calculadora científica en Python

![](IMG/3.PNG)

#### Implementación de una interfaz HMI en NODE-RED

![](IMG/11.PNG)




## 9. EXPLICACION DEL CODIGO FUENTE

### Para ver el codigo fuente de cada proyecto, este mismo se encuentra en la carpeta de CODIGO FUENTE


#### Diseño una calculadora científica en Python

Una vez realizada toda la explicación de nodos-red se procederá a realizar un ejercicio para crear un dashboard o una interfaz gráfica en la cual el usuario puede interactuar. Para empezar, se utilizará la biblioteca llamada “dashboard” por lo general está a viene instalada, pero, si es el caso de que no se posee la biblioteca se recomienda ir a la parte menú buscar la opción “manage paleta” e instalar la librería dashboard. 

La práctica que se va realizar consta de la elaboración de una casa, la cual posee 5 cuartos: dos dormitorios, una cocina, una ducha y un garaje, algo característico entre todas las habitaciones (con excepción del baño) es que poseen  focos o la luz. Se estableció en 5 flow´s al igual que se crearon 5 tabs, debido a que cada una de ellas viene a representar uno de los dormitorios.

Para elaboración del bombillo, se utilizó dos nodos “buttom” como entrada, estos representaran el estado del foco, es decir si va a estar encendido o apagado; se lo conectó con el nodo de salida “text” qué indica cuál es el estado del foco mostrando la elección del usuario en la interfaz.
Cómo se mencionó anteriormente la mayoría de los cuartos constan de focos es por ello que se inició con dicho grupo no obstante cada uno de los dormitorios poseen unas cualidades las cuales serán nombradas a continuación: 

En el primer dormitorio, por medio de un “slider” o deslizador y el nodo “gauge” se creó un medidor de volumen de música y por medio de una gráfica se analiza el volumen en función del tiempo y los niveles que se alcanza.

En el dormitorio matrimonial, se creó e implementó una gráfica que muestra la intensidad de luz que emite el foco además, se colocó luces led las cuales pueden variar el color de los leds con el utilizó del nodo “color picker” el cual muestra el color que el usuario desee obtener, para la iluminación se empleó adicionalmente un nodo “dropdown” que permite iluminar únicamente la parte izquierda (lámpara	),derecha(foco) o ambas. 

El tercer cuarto consta de la cocina, para ello se ha implementado una cocina automática la cual por medio de un nodo de “deslizador” y “buttom” permite que la cocina  encienda o se apague adicionalmente con un nodo “gauge” se nivelara el control de fuego que emite una hornilla.

Para el cuarto de la ducha se utilizó, dos nodos “buttom” que van a determinar si el agua va a estar fría y caliente los cuales están conectados con un nodo “text” el cual es el indicador de la temperatura que con ayuda de un nodo “switch” abrirá o cerrara el agua y un nodo gauge conectado con in “slider” para mostrar el nivel de agua qué va a salir.

En el garaje, la puerta será automática y se utilizará dos nodos “buttom” los cuales mostrarán si la puerta se abre o se cierra. Adicionalmente, se utilizará un nodo “audio out” el cual indicara la acción que realiza el “buttom” a través de un audio esto se aplicara en la segunda, tercera y quinta habitación. Finalmente para mostrar que se el usuario está generando una orden se mostrara una notificación que confirme la acción que va a realizar la interfaz para ello se utilizara un nodo llamado:”notifications” el cual va a estar conectado a cada “buttom” o “switch” aplicados.  


#### Implementación de una interfaz HMI en NODE-RED

En las 5 primeras líneas ingresas las librerías para utilizar las funciones del GPIO de los pines de la Raspberry, también la librería para las funciones matemáticas math, etc. Luego inicializamos 15 pines que son desde el 8 hasta el 38 para que se ha el ingreso de las operaciones, los siguientes 3 pines que son el 3, 5 sirven para el ingresó de datos, el 7 es para salir del ingreso de datos y 21 es para seleccionar la función de ingreso de datos en decimales, y por ultimo el pin 19 es para salir del programa. Ya inicializados los pines que vamos a utilizar la clase que es llamada la Calculadora, luego creamos los atributos, que son numero1, numero2, operación y opción.

Luego creamos el constructor y de creamos dos funciones para asignar valores a numero1, numero2, la siguiente función para cada operación matemática las cuales son las de una calculadora científica básica, la siguiente función sirva para leer la operación que se halla seleccionada mediante el ingreso de los pines, por lo cual utilizamos la función while e la función del if y eso cree un bucle y se pueda seguir seleccionando después y también sirve para imprimir el símbolo de cada operación, bien la función de leer número entero, que esta sirve para cuando no se halla seleccionada la opción del decimal que antes ya se había asignado el pin19, esta función se le ingresa los datos con los pines 3,5 y para salir el 7. 

Luego viene la función de ingreso de un numero decimal el cual funciona pidiéndote primero el numero entero y luego la parte decimal el cual también se ingresa con los pines 3,5,7.

La siguiente función es para imprimir los resultados por lo que llamamos a la función de operación que antes ya se había inicializamos anteriormente antes y la cual imprime dependiendo la operación, si es de ingreso de dos números imprime completo o sino imprime la parte del else el cual solo se debe ingresar un solo número, luego inicializamos la parte de operar el cual colocamos los pines a cada operación. Luego creamos la función menú que es para que imprima las operaciones con su pin para que pueda ingresar el usuario y al final llamamos a todos las funciones necesarias para que imprimamos el menú con while para crear un bucle hasta que el usuario quiera serrar el programa, luego creamos un if para cuando escoja si va hacer operaciones con decimal o con decimales, luego creamos una condicional para el factorial para que no se pueda ingresar decimales, luego creamos otra condición para que haga cierta operaciones puedan ingresar solo valor o ingrese los dosy al final la ante penúltima línea es para asignamos valores a los atributos de la clase, la penúltima es para que se realiza la operación relacionada y la última es para que imprima el resultado de la operación.




## 10. CONCLUSIONES

- La página https://create.withcode.uk/ la cual puedes crea funciones para ingresar y sacar datos, tiene muchas limitaciones de varias librerías y una de esas es la de librería SYS..
 
- Los nodos que nos ofrece NODE-RED son muy diversos, para poder tener otros nodos de los que vienen por determinado, se tienen que descargar. Pero no solo podemos encontrar nodos hechos por la misma plataforma, también podemos encontrar nodos hechos por usuarios, pero a veces estoy no están del todo bien hechos.

- En conclusión, podemos determinar que node red nos brinda una interfaz gráfica la cual, es amigable para el usuario inclusive para el desarrollo y el diseño del mismo al crear una dashboard debido a que se posee una lista de varios widgets preestablecidos los cuales se los puede  utilizar por la conexión entre nodos de entrada (bottom, dropdown,switch,color picker) lo que vamos a programar y los modos de salida (text, notification, audio out, gauge, chart) que vienen hacer lo que el usuario tiende a visualizar ;cada uno de estos posee parámetros en su configuración, en esta ocasión, se tomaron en cuenta los parámetros de label el cuál va a ser el nombre de nuestro nodo, playload que va a indicar la función que va a cumplir, range el cual crea un rango determinando los valores mínimos y máximos, graphics y colour.

- También podemos decir que la herramienta node red es muy potente y sirve para comunicar el hardware y los servicios de una forma rápida y sencilla simplificando en gran manera la programación del mismo; finalmente, se cumplió nuestro objetivo mediante la elaboración de un proyecto en dashboard el cual es el panel de una casa interactiva el cual era mostrar las elaboración un na dashboard.


 
## 11.RECOMENDACIONES

-	Al momento de instalar Node-red se debe tener en cuenta cual librería se va a instalar, se recomienda utilizar la realizada por Red-Note debido a que las demás son realizadas por usuarios y pueden tener funciones diferentes a las esperadas para esta práctica.

- Para poder realizar un programa en esta plataforma online hay que saber primero saber lenguaje Python, luego de ya tener los conocimentos vas al siguiente nivel el cual es la programacion dirigido objetos con plus de cono cimiento en activar los pines del Raspberry y poder hacer que se pueda ingresar o sacar datos. Estos pasos a sguir nos facilitara para crear mas facil cualquier proyecto relaccionado al mismo. 


 
## 12. CRONOGRAMA

![](IMG/crono.PNG)

 
 ## 13.BIBLIOGRAFÍA:

- Rupil, A. C., & García Mattío, M. (2019). Node-red, conectando cosas, apis y servicios en línea.

- Sánchez, M., Barrena, M., Bustos, P., Campillo, C., & García, P. (2016). Arquitectura software basada en tecnologías smart para agricultura de precisión. Jornadas de Ingeniería del Software y Bases de Datos.

- Oliphant, T. E. (2007). Python for scientific computing. Computing in Science & Engineering, 9(3), 10-20.

- Blackstock, M., & Lea, R. (2014, October). Toward a distributed data flow platform for the web of things (distributed node-red). In Proceedings of the 5th International Workshop on Web of Things (pp. 34-39).

- Lekić, M., & Gardašević, G. (2018, March). IoT sensor integration to Node-RED platform. In 2018 17th International Symposium INFOTEH-JAHORINA (INFOTEH) (pp. 1-5). IEEE.

-Tabaa, M., Chouri, B., Saadaoui, S., & Alami, K. (2018). Industrial communication based on modbus and node-RED. Procedia computer science, 130, 583-588.
 
 
## 14. ANEXOS

![](IMG/pi_board_pinout.jpg)

![](IMG/33.PNG)

![](IMG/primer.PNG)


 
## 15. MANUAL DE USUARIO

#### Diseño una calculadora científica en Python

1.	Descargar el WinRAR el cual se encuentra en los anexos con el nombre de CalculadoraCientifica.py.

![](IMG/Captura1.JPG)

2.	Luego extraer el archivo en el lugar donde quieres que este el archivo.

![](IMG/Captura2.JPG)

3.	Luego abrir el código con Bloc de notas.

![](IMG/Captura3.JPG)

4.	Abrir el navegador que usted prefiera, pero mejor si es el navegador Chrone.

![](IMG/Captura4.JPG)

5.	Luego abrir la pagina https://create.withcode.uk/ y copiar el código de la calculadora.

![](IMG/Captura5.JPG)

6.	Luego corres el programa y ya está.

![](IMG/2.PNG)


#### Implementación de una interfaz HMI en NODE-RED

1. Instalar Node.js en nuestra computadora el cual lo podemos encontrar en la pagina principal

![](IMG/111.png)

2. En el boton de a lupa en Windos escribiremos  "cmd" para abrir la pantalla de comandos.

![](IMG/444.jpeg)

3. Una vez abirta escribiremos el comando "node-red" seguido de un enter.

![](IMG/555.jpeg)
4. Se nos desplegara una serie de intruciones y una de ellas sera un direccion IP la cual copiaremos y pegaremos en nuestro navegador.

![](IMG/666.jpeg)

5. Cuando se acabe de cargar la plataforma  Node-RED aparecera y podremos trabajar con ella.

![](IMG/777.jpeg)

6. Para poder utilizar los nodos que nos permiitan trabajar en un dashboard necesitaremos descargar el paquete de estos nodos. Nos dirigiremos a la opcion de las tres lineas que se encuentra en la parte superior derecha.
![](IMG/0.jpeg)
7. Elegimos la opcion Manage Palette
![](IMG/00.jpeg)
8.  Escribimos “dashboard” y procedemos a instalar el primer paquete hecho por NODE-RED.
![](IMG/000.jpeg)

9. Ya instalado los nodo apareceran a la izquierda de nuestra pantalla, para poder tener un mejor manejo creremos diferentes TABS para poder trabajar de manera ordenada cada seccion de nuestra interfaz HMI.
![](IMG/888.jpeg)

10.Eligiremos los notos con los que queremos trabajar y los arrastraremos a la seccion del centro y para conectarlos bastaria con hacer clic en el recuadro blanco que esta a extremo de cada nodo.

![](IMG/999.jpeg)
11. Para finalizar hacemos clic  en Deploy para que la plataforma lo copile y acontinuacion hacemos clic en icono de una fecha para arriiba el cual nos permitira visualizar nuestro proyecto
![](IMG/11.PNG)
