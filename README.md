# 🤖 AI Recruiter Automator (n8n + Gemini)

Un sistema de automatización avanzado construido como un "Headhunter Virtual". Diseñado para eliminar las horas de trabajo manual en la revisión de currículums, extrayendo datos y evaluando candidatos de forma objetiva con Inteligencia Artificial.

## 🎯 El Problema que Resuelve
Los equipos de Adquisición de Talento pierden hasta un 60% de su tiempo leyendo currículums que no cumplen con los requisitos mínimos del puesto. Este proyecto automatiza el filtrado inicial, permitiendo a los reclutadores enfocarse en las entrevistas de valor.

## 📸 Arquitectura del Flujo
![Arquitectura del Flujo de n8n](flujo-n8n.png)

## 🚀 ¿Cómo funciona? (El Pipeline)

* **Fase 1: Ingesta y Pre-filtrado Parametrizable.** El flujo captura las postulaciones en tiempo real y ejecuta reglas de negocio para un descarte inmediato (MVP: validación de pretensión salarial). Esta capa de filtrado es 100% personalizable y escalable a cualquier criterio duro que requiera la vacante (ubicación, idioma, disponibilidad).
* **Fase 2: Lectura de Requisitos y Contexto de IA.** Para garantizar una evaluación precisa y a la medida de cada empresa, el flujo lee directamente desde Google Drive el perfil del puesto deseado. Esta arquitectura convierte al sistema en una herramienta completamente flexible: si el cliente necesita buscar un rol diferente mañana, solo tiene que actualizar el documento en su carpeta compartida, sin necesidad de que un programador modifique la automatización.
* **Fases 3 y 4: Consolidación y Entrega de Candidatos Ideales.** El sistema prepara automáticamente un reporte estructurado en Google Sheets que hereda la información clave de cada postulante. Actuando como un embudo de alta precisión, la automatización solo registra en este archivo final a los candidatos que aprueban los filtros estrictos definidos por el equipo de reclutamiento. Esto le entrega al reclutador una "Shortlist" (lista corta) inmaculada de talento viable, ahorrando horas de tabulación manual y revisión de perfiles no aptos.

## 🛠️ Stack Tecnológico
* **n8n:** Orquestación de flujos y manejo de APIs.
* **Google Gemini API:** Modelo LLM estructurado (cero alucinaciones).
* **Google Drive / Sheets API:** Almacenamiento y Base de Datos ligera.
* **JavaScript:** Manipulación y transformación de objetos JSON.

## 🚀 Próximos Pasos (Evolución del Producto)
* Integración con Telegram/WhatsApp para notificar al reclutador cuando un candidato de perfil "Alto" aplique.
* Generación de correos automáticos de rechazo o de invitación a entrevista.

---
**Desarrollado por:** [Tu Nombre]  
¿Conectamos? [Encuéntrame en LinkedIn](AQUI_PEGA_EL_LINK_DE_TU_LINKEDIN)

---
**Desarrollado por:** [Tu Nombre/Usuario]
¿Conectamos? [Encuéntrame en LinkedIn](AQUI_PEGA_EL_LINK_DE_TU_LINKEDIN)
