# Lectura de PDF Chatbot con Langchain y Streamlit
Este Chatbot es una aplicación interactiva desarrollada para interactuar con su PDF. Está construido utilizando Open Source Stack. 


<p align=center>
<img src="src\banner.png" height = 400 weight=500>
<p>

## Ejecución Local 💻

Siga estos pasos para configurar y ejecutar el proyecto en su máquina local.

### Instalación:

```bash
# Clonar el repositorio:
git clone <repository_url>
```

# Crear el entorno virtual :
```bash
python -m virtualenv venv
source venv/Scripts/activate
```


## Instalar las dependencias en el ambiente virtual :

```bash
pip install -r requirements.txt`
```

## Ejecutar la ingestion para la data:

```bash
python ingest.py
```
## Ejecutar chatbot application en Streamlit:

```bash
streamlit run chatbot_app.py
```

### Si tienes inconvenientes en la ingestion puedes ejecutar en PowerShell

## Crear el entorno virtual:
```sh
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process -Force 
./venv/Scripts/activate.ps1
```

## Ejecutar la ingestion para la data:

```sh
py ingest.py
```

## Para usar el modelo se necesita setear una variable y luego clonar:
```sh
GIT_LFS_SKIP_SMUDGE=1
git clone https://huggingface.co/MBZUAI/LaMini-T5-738M
```

## Ejecutar chatbot application en Streamlit:
```sh
streamlit run main.py -w
```