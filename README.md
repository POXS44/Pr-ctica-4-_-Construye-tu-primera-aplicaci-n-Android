# Solución _ Práctica 4 _ Construye tu primera aplicación Android


## REQUERIMIENTOS
###  Hardware
+ Computadora con los siguientes requisitos:
+ Procesador mínimo de velocidad de 2 GHz
+ Memoria RAM de 4 GB (recomendado 8 GB)    
+ Almacenamiento mínimo en disco de 2 GB (recomendado 4GB)
### Software
+ Android Studio  
+ Visual Studio Code  
+ JDK en cualquier versión
+ Windows 7/8/10 (64 bits)


## FUNCIONALIDAD
Esta práctica tiene como objetivo explorar el IDE Android Studio y crear su primera
aplicación Hola Mundo.

### ENUNCIADO
### I. Android Studio y Mi primer Hola Mundo
<img src="img\1.JPG"/>


## Tarea 1.1: Instalación de Android Studio
Android Studio proporciona un entorno de desarrollo integrado (IDE) completo,
incluido un editor de código avanzado y un conjunto de plantillas de aplicación. Además,
contiene herramientas para el desarrollo, depuración, pruebas y rendimiento que hacen
que sea más rápido y fácil desarrollar aplicaciones. Puedes probar tus aplicaciones con
una amplia gama de emuladores preconfigurados o en tu propio dispositivo móvil, crear
aplicaciones de producción y publicar en la tienda de Google Play.

Normalmente, esta tarea es un poco sencilla si ya tiene experiencia instalando programas
en cualquier sistema operativo, pero si tiene problemas al hacerlo siga la guía de
instalación de Android Studio de la documentación.
Después de la instalación compruebe lo siguiente, si le falta algo complete lo necesario:

### - Verifique que ya cuente con el JDK de Java en cualquier versión
<img src="img\2.png"/>

### -Verifique la ubicación de la instalación del SDK en Android Studio
<img src="img\3.JPG"/>

### -Verifique que en Android Studio este seleccionada la versión del JDK instalada en su máquina.



### Tarea 1.2: Crear la aplicación Hello World

### Crea el proyecto de aplicación

+ Estando en la ventana principal de Bienvenido a Android Studio, haga clic en
Iniciar un proyecto de Android Studio.

<img src="img\4.JPG"/>

+ Según la versión, es posible que primero seleccione la plantilla, entonces
seleccione una plantilla Empty Activity en el panel 
correspondiente a Phone y Tablet.

<img src="img\5.JPG"/>

o En la ventana de Configurar su proyecto, escriba Hello World para el nombre
de la aplicación

<img src="img\6.JPG"/>

o Compruebe la ubicación predeterminada del proyecto en donde desea almacenar
su aplicación, en el caso de que esa no sea su ubicación preferida, puede
cambiarla.
<img src="img\7.JPG"/>

o Si no tiene pensado publicar la aplicación, puede dejar el nombre del paquete
predeterminado.
<img src="img\8.JPG"/>

o En las nuevas versiones se elige Kotlin como el lenguaje de programación
predeterminado, en el caso de que no le aparezca seleccionado, establezca
Kotlin.
<img src="img\9.JPG"/>

o Indique que porcentaje de dispositivos usan la API nivel 19 y cuales son sus
características que incluye según el apartado Help me choose.

<img src="img\10.JPG"/>

### Caracteristicas
+ SELinux en modo estricto
+ Acceso al almacenamiento mejorado
+ Soporte para Bluetooth MAC
+ Dispositivos Buetooth podrán cambiar el volumen
+ Wi-Fi TDLS
+ WebView se pasa a Chromium
+ Framework para transiciones
+ Soporte para Infrarrojos
+ Impresión
+ Optimizado el consumo de la señal digital


+ De clic en finish, y espere que gradle sincronice todas las librerías necesarias
para su aplicación, esto puede tardar un momento, sea paciente.
+ Cada vez que inicia un proyecto le lanza un consejo del día, tome una captura
del consejo que le salió

<img src="img\Captura de pantalla (154).png"/>
<img src="img\Captura de pantalla (155).png"/>
<img src="img\Captura de pantalla (156).png"/>
<img src="img\Captura de pantalla (157).png"/>
<img src="img\Captura de pantalla (158).png"/>
<img src="img\Captura de pantalla (159).png"/>


### Aparece el editor de Android Studio

+ Haga clic en la pestaña activity_main.xml para ver el editor de diseño
<img src="img\11.JPG"/>

+ Haga clic en la pestaña Diseño del editor de diseño, si aun no está seleccionada,
para mostrar una representación gráfica del diseño como se muestra a
continuación.

<img src="img\Captura de pantalla (160).png"/>

+ Haga clic en la pestaña MainActivity.kt o MainActivity.java
<img src="img\12.JPG"/>


### Explore el proyecto en el panel Android

+ Si aún no está seleccionado, haga clic en la pestaña Proyecto en la columna de
la pestaña vertical en el lado izquierdo de la ventana de Android Studio. Aparece
el panel Proyecto. Explore todos sus directorios.

<img src="img\Captura de pantalla (161).png"/>

###  Explore la carpeta Gradle Scripts
El sistema de compilación Gradle en Android Studio facilita la inclusión de archivos
binarios externos u otros módulos de biblioteca en la compilación como
dependencias.

+ La primera vez que se crea un proyecto de aplicación, el panel Proyecto > Android
aparece con la carpeta Scripts de Gradle expandida como se muestra a continuación.

<img src="img\13.JPG"/>

o Si la carpeta Scripts de Gradle no está expandida, haga clic en el triángulo para
expandirla.  
+ Busque el archivo build.gradle (Project: Hello_World).

<img src="img\Captura de pantalla (162).png"/>

+ Busque el archivo build.gradle(Module:app).


<img src="img\Captura de pantalla (163).png"/>


### Explorar la aplicación y la carpeta res
Todo el código y los recursos de la aplicación se encuentran dentro de las carpetas
app y res.

+ Expanda la carpeta de la aplicación, la carpeta java y la carpeta
com.example.android.helloworld para ver el archivo java MainAc

<img src="img\14.JPG"/>


+ Expanda la carpeta res y la carpeta de diseño y haga doble clic en el archivo
activity_main.xml para abrirlo en el editor de diseño.
<img src="img\Captura de pantalla (164).png"/>


### Explorar la carpeta de manifiestos
o Expanda la carpeta de manifiestos.
o Abra el archivo AndroidManifest.xml.
o En cada uno de estos ficheros, indique para que se utilizan en el proyecto
Android

<img src="img\Captura de pantalla (165).png"/>



### Tarea 1.3: Use un AVD (Android Virtual Device)

Usará el administrador de dispositivos virtuales Android (AVD) para crear un
dispositivo virtual (también conocido como emulador) que simula la configuración de
un tipo determinado de dispositivo Android y usar ese dispositivo virtual para ejecutar la
aplicación.


###  Crear un dispositivo virtual de Android (AVD)
+ En Android Studio, seleccione Herramientas > Android > Administrador de
AVD o haga clic en el icono Administrador de AVD en la barra de
herramientas. Aparecerá la pantalla Sus dispositivos virtuales. Si ya ha creado
dispositivos virtuales, la pantalla los muestra (como se muestra en la figura
siguiente); de lo contrario se ve una lista en blanco.

<img src="img\16.JPG"/>


+  Haga clic en + Crear dispositivo virtual. Aparece la ventana Seleccionar
hardware que muestra una lista de dispositivos de hardware preconfigurados.
Para cada dispositivo, la tabla proporciona una columna para su tamaño de
visualización diagonal (Tamaño), resolución de pantalla en píxeles
(Resolución) y densidad de píxeles (Densidad).

<img src="img\17.JPG"/>

+ Haga clic en la pestaña Recomendado si aún no está seleccionada y elija qué
versión del sistema Android se ejecutará en el dispositivo virtual (como Pie).
<img src="img\18.JPG"/>


Hay muchas más versiones disponibles que las que se muestran en la
pestaña Recomendado. Mira las pestañas Imágenes x86 y Otras imágenes para verlas.
Si un vínculo de descarga está visible junto a una imagen del sistema que desea utilizar,
aún no está instalado. Haga clic en el vínculo para iniciar la descarga y haga clic
en Finalizar cuando haya terminado.


+ Ejecute la aplicación en el dispositivo virtual
o En Android Studio, elija Run > Ejecutar aplicación o haga clic en el
icono Ejecutar de la barra de herramientas.
<img src="img\Captura de pantalla (166).png"/>

+ En la ventana Seleccionar destino de implementación, en Dispositivos virtuales
disponibles, seleccione el dispositivo virtual que acaba de crear y haga clic en
Aceptar.

+ Este paso puede variar por si tiene un dispositivo predeterminado seleccionado

### Cuando finalice puede observar un resultado semejante al siguiente:

<img src="img\19.JPG"/>


## Ejecute la aplicación en un dispositivo físico

o Muestre todos los pasos necesarios para ejecutar su aplicación utilizando su
dispositivo físico


En el dispositivo fisico, dirijirse a Configuracion> Acerca del Telefono> Pulsar varias veces sobre el Numero de Compilacion hasta que muestre un mensaje que diga "Ya eres desarrollador"

Las opciones de desarrollador varian en dependencia al modelo del dispositivo .

o Encienda la depuración USB en su dispositivo físico

Luego dirijirse a las Opciones de Desarrollador previamente activadas, y dentro de ese menú buscar y activar el apartado de "Depuracion USB" .


<img src="img\20.jpg"/>
o Ejecute la aplicación en su dispositivo físico

<img src="img\21.jpg"/>


### Cambiar la configuración de Gradle de la aplicación

+ Cambiar la versión mínima del SDK para la aplicación

<img src="img\22.JPG"/>
<img src="img\23.JPG"/>
<img src="img\24.JPG"/>

+ Encuentre el fichero build.gradle (Module:app)

+ Busque la propiedad minSdkVersion a un nivel más bajo

+ Sincronice la nueva configuración de Gradle


<img src="img\25.JPG"/>

### Utilice instrucciones de Log para su aplicación


+ Ver el panel logcat y sus diferentes opciones de vista

<img src="img\26.JPG"/>


