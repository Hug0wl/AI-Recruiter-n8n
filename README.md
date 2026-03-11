# 🤖 AI Recruiter Automator (n8n + Gemini)

Un sistema de automatización avanzado construido como un "Headhunter Virtual". Diseñado para eliminar las horas de trabajo manual en la revisión de currículums, extrayendo datos y evaluando candidatos de forma objetiva con Inteligencia Artificial.

## 🎯 El Problema que Resuelve
Los equipos de Adquisición de Talento pierden hasta un 60% de su tiempo leyendo currículums que no cumplen con los requisitos mínimos del puesto. Este proyecto automatiza el filtrado inicial, permitiendo a los reclutadores enfocarse en las entrevistas de valor.

## 📸 Arquitectura del Flujo
*(Aquí va la imagen de cómo trabaja tu robot)*
![Arquitectura del Flujo de n8n](flujo-n8n.png)

## 🚀 ¿Cómo funciona? (Paso a Paso)
1. **Ingreso y Filtro:** El flujo detecta nuevos candidatos desde un formulario de Google Drive y hace un descarte inicial por pretensión salarial.
2. **Extracción (OCR):** Lee el documento PDF crudo y extrae todo el texto del currículum.
3. **Evaluación de IA Estricta:** Un nodo conectado a **Google Gemini** recibe el texto. Mediante un *prompt* estructurado, se le exige a la IA:
   - Evaluar años de experiencia reales.
   - No hacer suposiciones (si no está escrito, no lo sabe).
   - Devolver los datos en formato `JSON` puro.
4. **Exportación de Datos:** El JSON es limpiado y mapeado directamente a un Google Sheets, creando una base de datos tabulada y lista para tomar decisiones.

## 🛠️ Stack Tecnológico
* **n8n:** Orquestación de flujos y manejo de APIs.
* **Google Gemini API:** Modelo LLM estructurado (cero alucinaciones).
* **Google Drive / Sheets API:** Almacenamiento y Base de Datos ligera.
* **JavaScript:** Manipulación y transformación de objetos JSON.

## 🚀 Próximos Pasos (Fase 2)
* Integración con Telegram/WhatsApp para notificar al reclutador cuando un candidato de perfil "Alto" aplique.
* Generación de correos automáticos de rechazo o de invitación a entrevista.

---
**Desarrollado por:** [Tu Nombre/Usuario]
¿Conectamos? [Encuéntrame en LinkedIn](AQUI_PEGA_EL_LINK_DE_TU_LINKEDIN)
