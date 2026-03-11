# 🤖 AI Recruiter Automator (n8n + Gemini)

Sistema avanzado de automatización diseñado para actuar como un Headhunter virtual. Extrae datos de formularios, procesa currículums en PDF mediante OCR y utiliza Inteligencia Artificial (Google Gemini) para evaluar candidatos de forma objetiva contra un perfil de puesto, exportando los resultados limpios a Google Sheets.

## 🚀 Flujo de Trabajo (Workflow)

1. **Ingreso de Datos:** El candidato llena un formulario y adjunta su CV (PDF) en Google Drive.
2. **Loop & Aislamiento:** Un nodo iterativo aísla a cada candidato para garantizar la integridad de los datos durante la evaluación.
3. **Extracción de Texto:** Lectura profunda del documento PDF para extraer la experiencia y habilidades.
4. **Evaluación IA Estricta:** Un *prompt* de nivel de ingeniería obliga a Gemini a evaluar años de experiencia y conocimientos técnicos con **cero suposiciones** (si no está en el CV, no lo tiene).
5. **Estructuración de Datos:** La IA devuelve un objeto `JSON` puro y parseable.
6. **Mapeo y Exportación:** Los datos se cruzan matemáticamente y se envían a columnas específicas en Google Sheets para la toma de decisiones.

## 🛠️ Stack Tecnológico
* **n8n:** Orquestación, lógica del flujo y manejo de APIs (Workflows as Code).
* **Google Drive API:** Gestión y lectura de documentos.
* **Google Gemini API (1.5 Flash/Pro):** Modelo LLM estructurado para toma de decisiones sin alucinaciones.
* **Google Sheets API:** Base de datos ligera y visualización de resultados.
* **JavaScript:** Manipulación, formateo y limpieza de datos JSON dentro de la automatización.

## ⚙️ Cómo usar este proyecto
1. Importa el archivo `Plantilla_Publica.json` a tu instancia de n8n.
2. Configura tus propias credenciales de Google y Gemini API.
3. Reemplaza los campos `TU_ID_AQUI` en los nodos de Drive y Sheets con los IDs de tus propios documentos.

---
*Desarrollado como MVP (Fase 1) para la optimización de procesos de Selección y Adquisición de Talento.*