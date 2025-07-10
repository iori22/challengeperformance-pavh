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
