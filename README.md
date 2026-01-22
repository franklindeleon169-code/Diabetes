Diamond Diabetes AI 🩺🤖

Diamond Diabetes AI es una plataforma de predicción clínica integral (Full Stack) diseñada para estimar la progresión cuantitativa de la diabetes en pacientes. A diferencia de los sistemas binarios tradicionales, este sistema utiliza un modelo de Regresión Lineal para devolver un índice numérico de riesgo futuro basado en 10 variables clínicas.

🚀 Características principales

Predicción Cuantitativa: Estima la progresión de la enfermedad a un año basándose en biomarcadores fisiológicos.


Arquitectura Moderna: Backend asíncrono de alto rendimiento y Frontend reactivo.


Seguridad de Datos: Validación estricta de entradas médicas mediante Pydantic y TypeScript.

Interfaz de Usuario (UX): Diseño profesional con estética Glassmorphism para reducir la ansiedad del usuario.

🛠️ Stack Tecnológico

Inteligencia Artificial: Python, Scikit-Learn (Regresión Lineal), Joblib.


Backend: FastAPI (Python 3.11), Uvicorn.


Frontend: React, TypeScript, Vite.

Despliegue: Docker (Backend) y Vercel (Frontend).

📊 Variables de Entrada (Features)
El modelo analiza 10 variables clínicas fundamentales:

Edad

Sexo

BMI: Índice de masa corporal.

BP: Presión arterial media.

S1-S6: Seis mediciones de suero sanguíneo (TC, LDL, HDL, TCH, LTG, GLU).

💻 Instalación y Configuración
Backend (Python)
Navega al directorio backend/.

Crea un entorno virtual: python -m venv venv.

Activa el entorno e instala las dependencias:

Bash

pip install -r requirements.txt
Ejecuta el servidor de desarrollo:

Bash

python main.py
El servidor estará disponible en http://localhost:8000.

Frontend (React)
Navega al directorio frontend/.

Instala las dependencias:

Bash

npm install
Inicia el entorno de desarrollo:

Bash

npm run dev
🔌 API Endpoints
El backend expone los siguientes puntos de acceso principales:

GET /: Verifica el estado de la API y muestra métricas del modelo (MSE y R2).

POST /predict: Recibe un JSON con las 10 variables clínicas y devuelve la predicción de progresión.

📁 Estructura del Proyecto
/backend: Contiene el código de la API, el script de entrenamiento y los modelos serializados (.pkl).

/frontend: Contiene la aplicación React, componentes de UI y lógica de consumo de API.

/docs: Manuales de construcción paso a paso y diagramas de arquitectura.


Nota: Este proyecto ha sido desarrollado como parte del Curso Profesional: Desarrollo de Aplicaciones de IA Médica Full Stack.
