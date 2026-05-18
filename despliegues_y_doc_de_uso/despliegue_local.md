//por unica ves para crear el entorno
python -m venv .venv

//primero gitbash como admin
cd "C:\Users\simulador-unahur"

// desde la terminal de gitbash como admin cada ves que comenzamos un nuevo dia de trabajo.
// siempre trabajar con el entorno de trabajo 
source .venv/bin/activate

// luego ver si son necesarias las versiones puntuales de las librerias 
pip install -r requirements.txt

export TRANSICION_ADMIN_PASSWORD="clave-fuerte"  // 1234 para pruebas

// para correr la app en el navegador predeterminado
python -m streamlit run app.py --server.port 8502