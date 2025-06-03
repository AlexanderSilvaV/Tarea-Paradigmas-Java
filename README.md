🧪 Evaluación TAXDEBLOOM
Sistema de aplicación de pruebas basado en la Taxonomía de Bloom, desarrollado en Java con Swing. Permite aplicar pruebas interactivas, cargando ítems desde un archivo .txt y clasificando las preguntas según su nivel cognitivo.

📘 Descripción General
Este software fue desarrollado como parte del Trabajo II del curso Paradigmas de Programación. Implementa preguntas de selección múltiple y verdadero/falso, evaluando a los estudiantes según los niveles de la taxonomía cognitiva de Bloom.

🚀 Cómo iniciar el proyecto
⚠️ Importante:
El punto de entrada correcto del proyecto es la clase PantallaInicial.java, ubicada en frontend.vistas.

No debes ejecutar desde VentanaPreguntas.java, ya que inicialmente se intentaba cargar un .json, pero el formato válido es .txt.

🎯 Características principales
✅ Carga de ítems desde archivo .txt

✅ Navegación tipo wizard (una pregunta por pantalla)

✅ Registro de respuestas del usuario

✅ Cálculo de porcentajes por:

Nivel de la Taxonomía de Bloom

Tipo de ítem (selección múltiple o verdadero/falso)

✅ Revisión de ítems tras enviar la prueba

✅ Validación de formato y manejo de excepciones

⚠️ Problemas conocidos
La Pantalla Inicial puede no mostrarse correctamente en algunas resoluciones.
El botón “Ingresar” aparece desproporcionado respecto a la imagen de fondo.

Vista actual con desalineación:

🛠️ Recomendación: revisar el uso de LayoutManager y ajustar proporciones entre la imagen y los componentes (por ejemplo, usando GridBagLayout o diseño responsivo).

🗂️ Estructura del Proyecto
bash
Copiar
Editar
EvaluacionTAXDEBLOOM/
│
├── Resources/
│   ├── preguntas_evaluacion.txt      # Archivo principal de preguntas (formato válido)
│   ├── items_ejemplo.json            # No utilizado en la versión final
│
├── backend/
│   ├── controller/                   # Control de flujo de evaluación
│   ├── exceptions/                   # Excepciones personalizadas
│   ├── model/                        # Modelos de datos: ítems, evaluaciones, etc.
│   └── util/                         # Utilidades: lectura de preguntas, temporizador
│
├── frontend/
│   ├── componentes/                  # Componentes visuales reutilizables
│   ├── listeners/                    # Controladores de eventos (botones/menú)
│   └── vistas/                       # Interfaces principales: PantallaInicial, Opciones, etc.
│
├── img/                              # Recursos visuales de la GUI
│
├── txt/                              # Recursos adicionales (no críticos)
│
└── Main.java                         # Alternativa de entrada al programa
📄 Formato del archivo preguntas_evaluacion.txt
El archivo debe tener bloques de preguntas separados por una línea vacía. Cada bloque debe incluir:

markdown
Copiar
Editar
1. Tipo de ítem: seleccion_multiple | verdadero_falso
2. Pregunta
3. Opciones (solo si es selección múltiple), separadas por ;
4. Respuesta correcta
5. Nivel de Bloom
6. Tiempo estimado (segundos)
📌 Ejemplo:
Copiar
Editar
seleccion_multiple
¿Cuál es la capital de Francia?
París;Londres;Roma;Madrid
París
Recordar
30
👥 Integrantes del equipo
Felipe Arancibia

Franco Labarca

Javier Silva

