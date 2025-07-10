challengeperformance-pavh
Clona el repositorio o importalo

git clone https://github.com/iori22/challengeperformance-pavh.git
Recuerda debes estar en master!

*** Requisitos previos: Java JDK 8 o superior *** Verifica con: java -version Si no está instalado, descárgalo desde: https://www.oracle.com/java/technologies/javase-downloads.html o usa OpenJDK: https://adoptopenjdk.net/

Instalar JMETER
Paso 1: Descargar JMeter Ve al sitio oficial: https://jmeter.apache.org/download_jmeter.cgi Descarga la versión más reciente de Apache JMeter (zip o tgz) (no necesitas el código fuente).

Paso 2: Extraer el archivo Extrae el archivo ZIP/TGZ en el directorio donde desees instalar JMeter.

Paso 3: Establecer variables de entorno (opcional pero recomendado) Añade JAVA_HOME al path si aún no lo tienes configurado. En Windows, puedes hacerlo desde el Panel de control → Sistema → Variables de entorno.

Paso 4: Ejecutar JMeter Navega al directorio bin dentro de la carpeta de JMeter. Haz doble clic en: jmeter.bat para abrir la GUI.

Paso 5: Importar el proyecto New -> Open -> Buscar el proyecto -> Abrir: Thread Group.jmx

Paso 6: Ejecutar el proyecto

Antes de ejecutar se debe de modificar el componente Summary Report: cambiar esto "C:/Users/Anthony/OneDrive/Escritorio/Products-Add/resultados/tps100-AddProducts.csv" por una ruta de su maquina.
Finalmente presionar en Start.
Para generar el reporte seguir los siguientes pasos: reemplazar segun la ruta de su maquina jmeter -n -t ruta/del/archivo.jmx -l ruta/resultados.jtl -e -o ruta/reporte_html




Challenge Performance - PAVH
Repositorio: https://github.com/iori22/challengeperformance-pavh

Clonar el repositorio
git clone https://github.com/iori22/challengeperformance-pavh.git
cd challengeperformance-pavh
⚠️ Asegúrate de estar en la rama master.

Requisitos previos
☕ Java JDK 8 o superior
Verifica la instalación: java -version
Si no está instalado, puedes descargarlo desde:

Oracle JDK - OpenJDK (AdoptOpenJDK)

Instalación de Apache JMeter
Paso 1: Descargar JMeter
Accede al sitio oficial de JMeter y descarga la última versión: https://jmeter.apache.org/download_jmeter.cgi
Descarga la versión binaria (.zip o .tgz). No necesitas el código fuente.

Paso 2: Extraer el archivo
Extrae el archivo ZIP/TGZ en el directorio donde desees instalar JMeter.

Paso 3 (opcional): Configurar variables de entorno
Asegúrate de tener configurada la variable de entorno JAVA_HOME.

En Windows: Panel de control → Sistema → Configuración avanzada del sistema → Variables de entorno

Ejecutar JMeter
Paso 4: Iniciar JMeter
Navega a la carpeta bin dentro del directorio donde instalaste JMeter y ejecuta:

En Windows: Haz doble clic en jmeter.bat
En macOS/Linux: Ejecuta ./jmeter desde la terminal

Paso 5: Importar el proyecto .jmx
En JMeter GUI: File → Open -> Busca el archivo Thread Group.jmx incluido en este repositorio. -> Ábrelo.

Paso 6: Configurar ruta de resultados
Antes de ejecutar el test, modifica el componente Summary Report:
Reemplaza esta ruta:
C:/Users/Anthony/OneDrive/Escritorio/Products-Add/resultados/tps100-AddProducts.csv
Por una ruta válida en tu máquina local donde quieras guardar los resultados.

Paso 7: Ejecutar prueba
Haz clic en el botón Start (ícono de "play") para iniciar la prueba.

Generar Reporte HTML
Usa el siguiente comando en la terminal, reemplazando las rutas con las correspondientes a tu entorno:
jmeter -n -t ruta/al/archivo.jmx -l ruta/resultados.jtl -e -o ruta/reporte_html

-n: Ejecuta en modo no-GUI
-t: Ruta del archivo .jmx
-l: Ruta del archivo .jtl (resultados)
-e: Genera el reporte
-o: Directorio de salida del reporte HTML
