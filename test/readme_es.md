# 🚀 Herramienta de Análisis de Código Estático (vuln_analisis_tool)

Esta herramienta realiza un análisis estático del código utilizando `cppcheck` para identificar vulnerabilidades en proyectos C/C++.

## 📋 Descripción

Este contenedor Docker ejecuta un script que utiliza `cppcheck` para analizar el código fuente del proyecto montado y generar un reporte de vulnerabilidades.

## 🛠 Requisitos

- Docker instalado en tu sistema.

## 🚀 Uso

### 1. Construir la Imagen Docker

Primero, construye la imagen Docker con el siguiente comando:

```sh
docker build -t vuln_analisis_tool .
### 2. Ejecutar el Contenedor
Asegúrate de estar en el directorio que contiene el código fuente que deseas analizar. Luego, ejecuta el contenedor con:

docker run -it --rm -v $(pwd):/proyecto vuln_analisis_tool

📌 Notas
Asegúrate de que cppcheck esté instalado en tu máquina local si deseas usarlo fuera del contenedor.
El contenedor eliminará los archivos temporales generados durante el análisis al finalizar la ejecución.
