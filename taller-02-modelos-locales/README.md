# 🧪 Taller #2 - Corre tu primer modelo local sin GPU con `llama.cpp`

Este es un taller práctico de **Zenomy Labs**, donde mostramos cómo correr modelos de lenguaje open source directamente desde Google Colab, usando solo CPU y menos de 12 GB de RAM.

---

## 🎯 ¿Qué vas a aprender?

- Qué es `llama.cpp` y por qué es útil para correr modelos sin GPU.
- Cómo descargar y usar modelos `.gguf` compatibles.
- Cómo generar texto con `llama-cpp-python` desde un entorno sencillo.
- Cómo comparar calidad, velocidad y uso de recursos entre modelos pequeños.

---

## 🚀 ¿Por qué hacemos esto?

En Latinoamérica muchas veces no tenemos acceso a GPUs o infraestructura de alto nivel.  
Pero eso no nos impide **explorar, aprender y construir IA localmente**.

Este taller busca **democratizar la experimentación con LLMs** y mostrar que sí es posible hacer IA desde el sur del mundo.

---

## 🧰 Requisitos

- Cuenta de Google (para usar Google Colab).
- Curiosidad técnica.
- Nada de hardware especial.

---

## 📓 Accede al taller

👉 [Abrir notebook en Google Colab](https://colab.research.google.com/drive/1lPny_Ye9mhYq6ad0vD7V2ORuFO37YmJO?usp=sharing)

> Si el enlace está caído, puedes abrir directamente el archivo `notebook.ipynb` desde tu cuenta de Google Drive.

---

## 📦 Modelos sugeridos

Todos en formato `.gguf` y compatibles con `llama.cpp`:

- [`Qwen3-1.7B`](https://huggingface.co/unsloth/Qwen3-1.7B-GGUF)
- [`TinyLlama 1.1B`](https://huggingface.co/TheBloke/TinyLlama-1.1B-Chat-v1.0-GGUF)
- [`Gemma 2B`](https://huggingface.co/TheBloke/gemma-2b-it-GGUF) (requiere más RAM)

---

## 🧪 Ejemplo mínimo

```python
from llama_cpp import Llama

llm = Llama(model_path="models/Qwen3-1.7B-GGUF.gguf", n_ctx=512, n_threads=4)
output = llm("¿Qué es la inteligencia artificial?", max_tokens=100)
print(output['choices'][0]['text'].strip())
```

🧠 Sobre Zenomy Labs
Zenomy Labs es una iniciativa abierta para impulsar la IA desde LATAM.
Creemos en aprender en público, compartir lo que hacemos y construir comunidad.

📎 https://zenomyai.com
📢 @zenomy_ai en Instagram

🤝 Contribuye o comparte
¿Probaste otros modelos? ¿Hiciste mejoras al notebook?
¡Haz un fork, súbelo a redes o manda PR!
