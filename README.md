# ==========================================================
# MEMORÁNDUM DE DEPENDENCIAS - PROYECTO TRANSICIÓN ACADÉMICA
# ==========================================================
# pip install --only-binary :all: pandas streamlit sqlalchemy pyyaml reportlab
# pip install plotly
# Instalación de dependencias (Estrategia de Binarios para evitar errores de compilación)



# 1. STREAMLIT (v1.36.0)
# Es el núcleo de la aplicación. Maneja tanto el servidor web como 
# la interfaz de usuario (Frontend). Permite crear botones, selectores 
# y tablas interactivas usando solo lógica de Python.
import streamlit as st

# 2. PANDAS (v2.2.2)
# La herramienta principal para manipulación de datos. Se usa para 
# procesar las listas de alumnos, equivalencias de materias y los 
# nuevos planes de estudio en formato de tablas (DataFrames).
import pandas as pd

# 3. SQLALCHEMY (v1.4.52)
# El "traductor" entre Python y la base de datos. Permite realizar 
# consultas SQL de forma segura y eficiente para persistir la 
# información de la transición académica.
import sqlalchemy as db

# 4. REPORTLAB (v4.2.2)
# Motor de generación de documentos. Se utiliza para crear los 
# certificados de equivalencia o reportes analíticos en formato PDF 
# que los estudiantes o directivos pueden descargar.
from reportlab.pdfgen import canvas

# 5. PYYAML (v6.0.2)
# Manejador de archivos de configuración (.yaml). Ideal para guardar 
# parámetros del sistema (como nombres de facultades o rutas de red) 
# fuera del código fuente, facilitando el mantenimiento.
import yaml

# ==========================================================