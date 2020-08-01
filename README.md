# raspberry-sensor-veml6070

Repositorio con modelo y ejemplos para el sensor VEML6070 que obtiene valores UV de la luz en el ambiente.

Para el funcionamiento del sensor se parte de la librería oficial de adafruit:

https://github.com/adafruit/Adafruit_CircuitPython_VEML6070

https://learn.adafruit.com/adafruit-veml6070-uv-light-sensor-breakout/python-circuitpython

De forma que este repositorio utiliza esa librería y sus dependencias como base
añadiendo otras características que he visto necesarias en mi caso.

## Dependencias

Los entornos donde han sido probados satisfactoriamente utilizaban las 
siguientes versiones de las aplicaciones necesarias:

- python 3.7.3
- raspbian, basado en debian 10.1
- bash 5.0.3 
- pip3 18.1

Se tiene que instalar la librería de adafruit mediante el gestor de paquetes de
python 3

```bash 
pip3 install adafruit-circuitpython-veml6070
```

También puedes adaptarlo usando entornos virtuales o descargar el repositorio
manualmente desde el enlace indicado al comienzo de este documento.

## Tabla de comparción por índice uv

Índice UV 	        ½T → 56,25 ms 	1T → 112,5 ms 	2T → 225 ms     4T → 450 ms
Bajo. De 0 a 2 	    0-280 	        0-560 	        0-1120 	        0-2240
Moderado. De 3 a 5 	281-560 	    561-1120 	    1121-2241 	    2241-4482
Alto. De 6 a 7 	    561-747 	    1121-1494 	    2242-2988 	    4483-5976
Muy alto. De 8 a 10 748-1027 	    1495-2054 	    2989-4108 	    5977-8216