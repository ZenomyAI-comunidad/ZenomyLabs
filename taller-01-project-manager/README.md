# 🧠 Taller 01 – Presupuestador automático de proyectos con IA

Este taller te guía paso a paso para construir un sistema que convierte **una idea de proyecto** (por ejemplo, "una app de reservas para eventos comunitarios") en una **descripción técnica + stack sugerido + presupuesto estimado por ítem**.

### ⚙️ ¿Qué hace?

Con solo escribir una idea o requerimiento, este sistema:

1. Valida si la idea es presupuestable
2. Genera una descripción estructurada del proyecto
3. Sugiere tareas o componentes técnicos
4. Estima cantidades, precios y subtotales (en USD)

> Todo esto usando **Gemini Pro** (Google), **LangChain**, y procesamiento básico en Python.

---

## 🛠️ Tecnologías usadas

- Google Generative AI (Gemini)
- LangChain (con Output Parsers y Chains)
- Pydantic (validación estructurada)
- Google Colab (para fácil ejecución)

---

## 🚀 ¿Cómo probarlo?

1. Abre este notebook en Google Colab:  
   [[Abrir en Colab]](https://colab.research.google.com/drive/1Bisce-f_rokc6q_cqTdcOH9TpKcDrKJ7)

2. Completa tu API key de Gemini (es gratis)

3. Escribe una idea simple como:  
   `"Una plataforma para gestionar préstamos de libros entre vecinos"`

4. Ejecuta el flujo y observa cómo genera un presupuesto completo.

---

## 📦 Archivos

- `project_manager_colab.ipynb`: notebook principal
- `App de Alquiler de Canchas de Fútbol.pdf`: vista previa del resultado
- `README.md`: este archivo

---

## 📍¿Por qué hicimos esto?

Queremos mostrar cómo los modelos de lenguaje pueden ayudar a crear herramientas reales, no solo chatbots.

Este es el primer taller de **Zenomy Labs**, una serie de guías abiertas donde compartimos prototipos funcionales, pensados para ser el punto de partida de productos más grandes.

---

## 💬 ¿Tienes una idea que te gustaría automatizar?

Abrimos la conversación:
- [@zenomy_ai](https://www.instagram.com/zenomy_ai)
- [LinkedIn](https://www.linkedin.com/company/zenomy_ai)
- O deja un issue con tu idea 🚀

---

Con ❤️ desde Latinoamérica.  
**Zenomy – IA que construye.**
