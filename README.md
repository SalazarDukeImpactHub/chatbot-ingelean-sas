# Proyecto Chatbot para INGE LEAN S.A.S

Este repositorio contiene los recursos y el código fuente del proyecto de chatbot desarrollado para INGE LEAN S.A.S., una solución de inteligencia artificial diseñada para mejorar la atención al cliente.

## 🚀 Visión General del Proyecto

El objetivo principal de este proyecto es implementar un chatbot inteligente capaz de ofrecer respuestas automáticas, personalizadas y rápidas a las preguntas frecuentes de los clientes de INGE LEAN S.A.S. El chatbot está construido para ser un asistente adaptativo, con capacidades de análisis, trazabilidad de interacciones y un mecanismo de aprendizaje incremental que le permite evolucionar y mejorar con el tiempo.

### Características Clave:

* **Respuestas automáticas y personalizadas:** Brinda información relevante y adaptada a cada usuario.
* **Rapidez:** Las respuestas se entregan en menos de 2 segundos.
* **Alta cobertura:** Cubre al menos el 90% de las preguntas frecuentes.
* **Manejo multiusuario:** Capacidad para atender a múltiples usuarios simultáneamente.
* **Trazabilidad de interacciones:** Registro y seguimiento de todas las conversaciones.
* **Comprensión Semántica:** Utiliza `sentence-transformers` para entender el significado de las preguntas, incluso si están formuladas de diferentes maneras.
* **Aprendizaje Incremental:** El modelo se puede re-entrenar con nuevas interacciones para mejorar continuamente.

## 🔗 Enlaces Importantes

* **Presentación del Proyecto (Canva):**
    https://www.canva.com/design/DAGuUoiV7kM/NaAH41r44cCHormGDsjZwQ/view?utm_content=DAGuUoiV7kM&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=ha869b4581e

* **Chatbot en Telegram:**
    https://t.me/TalentoTech_InGeleanSASchat_bot

## 📁 Estructura del Repositorio

El repositorio está organizado de la siguiente manera:
.
├── Modelos/
│   ├── chatbot_model.pkl
│   └── tfidf_vectorizer.pkl
├── INGE LEAN S.A.S - Procesador.blueprint.json
├── INGE LEAN S.A.S - Procesador.png
├── INGE LEAN S.A.S El Recepcionista.blueprint.json
├── INGE LEAN S.A.S El Recepcionista.png
├── chatbot_project.pdf
└── README.md

### Contenido de las Carpetas y Archivos:

* **`Modelos/`**:
    * `chatbot_model.pkl`: Contiene el modelo de Machine Learning entrenado (Regresión Logística) para la clasificación de intenciones.
    * `tfidf_vectorizer.pkl`: Contiene el vectorizador TF-IDF utilizado para transformar el texto de las preguntas en un formato numérico que el modelo pueda entender.

* **`INGE LEAN S.A.S - Procesador.blueprint.json`**:
    * Archivo blueprint de Make.com que define el escenario del "Procesador de Habilidades". Este escenario se encarga de recibir las preguntas del usuario, enviarlas a la API de Flask, y procesar la respuesta generada por el modelo de IA.

* **`INGE LEAN S.A.S - Procesador.png`**:
    * Captura de pantalla del flujo del "Procesador de Habilidades" en Make.com, mostrando la interconexión de módulos como el inicio del subescenario, la solicitud HTTP a la API y la integración con OpenAI.

* **`INGE LEAN S.A.S El Recepcionista.blueprint.json`**:
    * Archivo blueprint de Make.com que define el escenario principal del chatbot "El Recepcionista". Este escenario gestiona la interacción con Telegram, enruta los mensajes y coordina las respuestas de bienvenida o el procesamiento de habilidades.

* **`INGE LEAN S.A.S El Recepcionista.png`**:
    * Captura de pantalla del flujo del chatbot "El Recepcionista" en Make.com, ilustrando cómo se reciben las actualizaciones de Telegram, se enrutan los mensajes y se envían las respuestas.

* **`chatbot_project.pdf`**:
    * Documento PDF que detalla el proyecto del chatbot, incluyendo la visión del reto, los resultados esperados, los bloques de código para la preparación del dataset, entrenamiento del modelo, visualización de métricas, mecanismo de aprendizaje incremental y la configuración de la API REST con Flask. Este documento proporciona una visión técnica profunda del desarrollo.

## 🛠️ Tecnologías Utilizadas

* **Python:** Lenguaje de programación principal para el desarrollo del modelo y la API.
* **Scikit-learn:** Librería para Machine Learning (TF-IDF, Naive Bayes, Regresión Logística).
* **Sentence-transformers:** Para la comprensión semántica y el manejo de paráfrasis.
* **Flask:** Microframework para la creación de la API REST.
* **Make.com (anteriormente Integromat):** Plataforma de automatización para la integración del chatbot con Telegram y la orquestación de los flujos de trabajo.
* **Telegram API:** Para la interacción con los usuarios a través de la plataforma de mensajería.
* **OpenAI GPT-4o:** Utilizado para la generación de respuestas y la gestión de la conversación.

## 🚀 Cómo Empezar

Para replicar o contribuir a este proyecto, puedes:

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/tu-usuario/nombre-del-repositorio.git](https://github.com/tu-usuario/nombre-del-repositorio.git)
    cd nombre-del-repositorio
    ```
2.  **Instalar las dependencias de Python:**
    (Se recomienda crear un entorno virtual)
    ```bash
    pip install -r requirements.txt # (Necesitarás crear este archivo con las dependencias)
    ```
3.  **Configurar y ejecutar la API de Flask:**
    Consulta el archivo `chatbot_project.pdf` para los pasos detallados sobre cómo cargar el modelo y el vectorizador, y ejecutar la aplicación Flask.
4.  **Importar los blueprints de Make.com:**
    Importa los archivos `.blueprint.json` en tu cuenta de Make.com para configurar los escenarios de "El Recepcionista" y el "Procesador de Habilidades". Asegúrate de configurar las conexiones necesarias (Telegram, OpenAI, y la URL de tu API de Flask).

---

¡Esperamos que este proyecto sea de gran utilidad y contribuya a mejorar la eficiencia de la atención al cliente en INGE LEAN S.A.S.!

