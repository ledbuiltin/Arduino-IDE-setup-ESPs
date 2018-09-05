# Arduino-IDE-setup-ESPs

ESP8266
Descargar ultimo IDE arduino: https://www.arduino.cc/en/Main/Software
Instalar driver CH340: https://sparks.gogo.co.nz/ch340.html
File/Preferences: http://arduino.esp8266.com/stable/package_esp8266com_index.json
Boardmanager ESP8266
Restart aduino

ESP32
Instrucciones: https://github.com/espressif/arduino-esp32/blob/master/docs/arduino-ide/windows.md
Video Youtube:https://www.youtube.com/watch?v=Odh0LWXOZZk&ab_channel=SinapTec
              o del tio con acento suizo
Ojo que el driver USB podria ser el CP2102
Descargar Git GUI: https://git-scm.com/download/win
Instalarlo acptando todo
Abrir y darle a clonar repositorio
Source: https://github.com/espressif/arduino-esp32.git
Target: C:\Users\david_barriuso\Documents\Arduino\hardware\espressif\esp32    */ ojo que no son barras hacia delante como viene en el ejemplo
Abrimos Git bash (que es como una ventanita en linea de comandos de Linux)
Accedemos al directorio C:/Users/david_barriuso/Documents/Arduino/hardware/espressif/esp32
Si abrimos Git bash desde git GUI ya va por defecto a esa carpeta
Es decir cd C:/Users/david_barriuso/Documents/Arduino/hardware/espressif/esp32
Ejecutamos (es decir pegar + enter)  git submodule update --init --recursive
Vamos a la carpeta C:/Users/david_barriuso/Documents/Arduino/hardware/espressif/esp32/tools y ejecutamos get.exe esto crea unas carpetillas es instala el compilador para el ESP32 (mientas aparece una ventana de comando diciendo que descarga algo, estrae, descarga, instala y se cierra sola)
Reiniciamos arduino y ya aparecen en el board manager unas cuantas ESP32
Parece que hay que tener descargado Python tambien... https://www.python.org/downloads/ yo he metido la 3.7
Hace falta Python porque los programillas que se instalan al ejegutar get.exe corren en Python

Para ver si el repositorio esta actualizado:
Abrimos Git GUI y vamos a Abrir reciente
Remote/ Fetch from/origin
En C:/Users/david_barriuso/Documents/Arduino/hardware/espressif/esp32/tools y ejecutamos get.exe como habiamos hecho antes durante la instalacion
