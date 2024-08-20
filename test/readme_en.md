# 🚀 Static Code Analysis Tool (vuln_analisis_tool)

This tool performs static code analysis using `cppcheck` to identify vulnerabilities in C/C++ projects.

## 📋 Description

This Docker container runs a compiled script that uses `cppcheck` to analyze the source code of the mounted project and generate a vulnerability report.

## 🛠 Requirements

- Docker installed on your system.
- Access to Docker Hub to pull the image.

## 🚀 Usage

### 1. Pull the Docker Image

First, pull the Docker image from Docker Hub with the following command:

docker pull cmvgg/vuln_analisis_tool

### 2. Run the Container

Make sure you are in the directory containing the source code you want to analyze. Then, run the container with:

docker run -it --rm -v $(pwd):/proyecto cmvgg/vuln_analisis_tool

3. Interaction

The script will prompt you for the project path inside the container (which should be /proyecto), and then generate a vulnerability report in the mounted directory.

📌 Notes

The container will remove temporary files generated during the analysis upon completion.