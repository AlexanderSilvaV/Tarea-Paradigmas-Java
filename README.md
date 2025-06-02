# Evaluación TAXDEBLOOM

Sistema de aplicación de pruebas según la Taxonomía de Bloom, desarrollado en Java utilizando Swing. Permite cargar ítems de evaluación desde archivo `.txt`, aplicar pruebas interactivas y revisar resultados según nivel cognitivo y tipo de pregunta.

## 📚 Descripción

Este software fue creado como parte del Trabajo II del curso **Paradigmas de Programación**. Utiliza los niveles de la Taxonomía de Bloom para clasificar preguntas de selección múltiple y verdadero/falso, y permite aplicar evaluaciones a estudiantes.

## 🧠 Características principales

- Carga de ítems desde archivo `.txt`.
- Visualización interactiva tipo wizard (una pregunta por pantalla).
- Navegación entre preguntas (anterior/siguiente).
- Registro de respuestas del usuario.
- Cálculo de porcentajes de respuestas correctas por:
  - Nivel de la Taxonomía de Bloom.
  - Tipo de ítem (selección múltiple o verdadero/falso).
- Revisión de ítems después de enviar la prueba.
- Validación de formato de archivo y control de excepciones.

## 🗃️ Estructura del Proyecto

- `backend/`: lógica y modelos.
- `frontend/`: interfaz gráfica (Java Swing).
- `Resources/`: archivos de prueba (`preguntas_evaluacion.txt`).
- `img/`: imágenes utilizadas en la interfaz.
- `txt/`: recursos adicionales.

## 📂 Formato del archivo de ítems (`preguntas_evaluacion.txt`)

El formato del archivo `.txt` consiste en bloques de preguntas, separados por líneas vacías. Cada bloque contiene:

1. Tipo de ítem (`seleccion_multiple` o `verdadero_falso`)
2. Pregunta
3. Opciones (solo para selección múltiple), separadas por punto y coma (`;`)
4. Respuesta correcta
5. Nivel de Bloom
6. Tiempo estimado (en segundos)

**Ejemplo:**
