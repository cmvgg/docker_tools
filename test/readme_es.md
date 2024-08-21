# 🚀 Herramienta de Análisis de Código Estático (vuln_analisis_tool)

Esta herramienta realiza un análisis estático del código utilizando `cppcheck` para identificar vulnerabilidades en proyectos C/C++.

## 📋 Descripción

Este contenedor Docker ejecuta un script compilado que utiliza `cppcheck` para analizar el código fuente del proyecto montado y generar un reporte de vulnerabilidades.

## 🛠 Requisitos

- Docker instalado en tu sistema.
- Acceso a Docker Hub para descargar la imagen.

## 🚀 Uso

### 1. Descargar la Imagen Docker

Primero, descarga la imagen Docker desde Docker Hub con el siguiente comando:

docker pull cmvgg/vuln_analisis_tool

### 2. Ejecutar el Contenedor
Asegúrate de estar en el directorio que contiene el código fuente que deseas analizar. Luego, ejecuta el contenedor con:

docker run -it --rm -v $(pwd):/proyecto cmvgg/vuln_analisis_tool

### 3. Interacción
El script generará un reporte de vulnerabilidades en el directorio montado.

📌 Notas

El contenedor eliminará los archivos temporales generados durante el análisis al finalizar la ejecución.