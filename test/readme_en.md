
# 🚀 Static Code Analysis Tool (vuln_analisis_tool)

This tool performs static code analysis using `cppcheck` to identify vulnerabilities in C/C++ projects.

## 📋 Description

This Docker container runs a script that uses `cppcheck` to analyze the source code of the mounted project and generate a vulnerability report.

## 🛠 Requirements

- Docker installed on your system.

## 🚀 Usage

### 1. Build the Docker Image

First, build the Docker image with the following command:

```sh
docker build -t vuln_analisis_tool .

### 2. Run the Container

Make sure you are in the directory containing the source code you want to analyze. Then, run the container with:

docker run -it --rm -v $(pwd):/proyecto vuln_analisis_tool


### 3. Interaction

The script will prompt you for the project path inside the container (which should be /proyecto), and then generate a vulnerability report in the mounted directory.

📌 Notes

Ensure cppcheck is installed on your local machine if you want to use it outside the container.
The container will remove temporary files generated during the analysis upon completion.