# 🤖 TalentBot: AI Recruiter Automator (n8n + Gemini)

Un sistema de automatización avanzado construido como un "Headhunter Virtual". Diseñado para eliminar las horas de trabajo manual en la revisión de currículums, extrayendo datos y evaluando candidatos de forma objetiva con Inteligencia Artificial.

## 📊 El Impacto: Humano vs. Máquina
Los equipos de Adquisición de Talento pierden hasta un 60% de su tiempo leyendo currículums que no cumplen con los requisitos mínimos del puesto. 

Según estudios de la industria de Recursos Humanos, un reclutador hace un escaneo visual de 7 segundos, pero realizar una **evaluación técnica y profunda** cruzando un CV contra el perfil del puesto le toma a un humano entre **4 a 5 minutos por candidato**.
* 🧑‍💼 **Humano:** Evaluar 10 CVs a detalle toma entre **40 y 50 minutos**.
* 🤖 **TalentBot:** Audita, cruza datos y evalúa **10 CVs cada 4 minutos**. 

## 🧪 Validación y Eficacia del Sistema
Esta primera etapa del sistema está diseñada para aplicar **filtros crudos y estrictos** sobre grandes volúmenes de candidatos. 
Para validar su precisión, el sistema ha sido sometido a **7 pruebas de estrés procesando más de 600 CVs reales**. El resultado demostró una **tasa de acierto del 87%** en sus evaluaciones al ser comparado con el criterio de revisión de un Headhunter Senior humano.

## 🧠 El "Cerebro": Prompt Engineering Avanzado
El núcleo de la toma de decisiones de TalentBot no es un simple chat, sino un **Prompt Maestro altamente específico e instruccional**. 
* **100% Modificable:** El prompt puede ser ajustado para cambiar la "personalidad" o la rigurosidad del evaluador según la vacante.
* **Cero Suposiciones:** Está programado con reglas de "Anclaje de Datos" que le prohíben a la IA deducir o inventar habilidades que no estén escritas literalmente en el CV, eliminando el sesgo y las alucinaciones.

## 📸 Arquitectura del Flujo
![Arquitectura del Flujo de n8n](flujo-n8n.png)

## 🚀 ¿Cómo funciona? (El Pipeline)

* **Fase 1: Ingesta y Filtro Crudo Parametrizable.** El flujo captura las postulaciones en tiempo real y ejecuta reglas de negocio para un descarte crudo e inmediato (MVP: validación de pretensión salarial, ubicación, idioma). Esta capa es la primera barrera de contención contra el spam de postulaciones.
* **Fase 2: Lectura de Requisitos y Análisis de IA.** El flujo lee directamente desde Google Drive el perfil del puesto deseado y lo cruza con el CV del candidato usando nuestro Prompt Maestro. Esta arquitectura es completamente flexible: si el cliente necesita buscar un rol diferente mañana, solo actualiza el documento en su Drive, sin necesidad de tocar el código de automatización.
* **Fases 3 y 4: Consolidación y Entrega de la "Shortlist".** El sistema actúa como un embudo de alta precisión, limpiando la estructura de datos (JSON) y preparando automáticamente un reporte en Google Sheets. El reclutador recibe un archivo final inmaculado, tabulado con puntajes cuantitativos y conclusiones de la IA, ahorrando horas de revisión de perfiles no aptos.

## 🛠️ Stack Tecnológico
* **n8n:** Orquestación de flujos y manejo de APIs.
* **Google Gemini API:** Modelo LLM estructurado y análisis documental.
* **Google Drive / Sheets API:** Almacenamiento y Base de Datos ligera.
* **JavaScript:** Manipulación, depuración y transformación de objetos JSON.

## 🚀 Próximos Pasos (Evolución del Producto)
* Integración con Telegram/WhatsApp para notificar al reclutador inmediatamente cuando aplique un candidato con "Puntaje Excepcional".
* Generación de correos automáticos de rechazo o de invitación a entrevista.

---
**Desarrollado por:** Nestor Hugo Huanca G  
¿Conectamos? [Encuéntrame en LinkedIn](https://www.linkedin.com/in/nestorhuanca/)
