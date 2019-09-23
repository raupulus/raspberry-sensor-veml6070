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