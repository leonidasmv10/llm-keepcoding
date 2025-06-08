# 🦕 Chatbot de Animales Prehistóricos

Este proyecto consiste en un **chatbot educativo** especializado en **animales prehistóricos**, potenciado con inteligencia artificial. Responde con **expresiones españolas**.

---

## 🔧 Tecnologías Utilizadas

- 🧠 **Modelo base**: [`Qwen2.5-3B-Instruct`](https://huggingface.co/Qwen/Qwen2.5-3B-Instruct)  
- 📚 **Fine-tuning**: realizado con [LlamaFactory](https://github.com/hiyouga/LLaMA-Factory)  
- 🗂️ **Dataset personalizado**: [`spanish-accent-dataset`](https://huggingface.co/datasets/leonidasmv/spanish-accent-dataset)  
- 🎨 **Generación de imágenes**: [`stable-diffusion-xl-base-1.0`](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)  
- 🔎 **Mejora de respuestas**: Sistema RAG usando **ChromaDB**  
- 🧠 **Detector de intención**: clasifica la intención del usuario para adaptar la respuesta  
- 🤖 **Gemini**: usado para simular batallas y detectar intenciones complejas  
- 💬 **Interfaz de prueba**: Google Colab  

---

## 🏗️ Estructura del Proyecto

### 1. Dataset

Se creó un dataset propio con ejemplos de conversación en español peninsular, incluyendo expresiones coloquiales, modismos y entonaciones características del habla española.

🔗 [leonidasmv/spanish-accent-dataset](https://huggingface.co/datasets/leonidasmv/spanish-accent-dataset)

### 2. Fine-tuning

El modelo `Qwen2.5-3B-Instruct` fue afinado usando **LlamaFactory**, logrando adaptar la personalidad española al modelo.

🔗 [qwen2.5-3b-instruct-spanish-accent-finetuning](https://huggingface.co/leonidasmv/qwen2.5-3b-instruct-spanish-accent-finetuning)

> ⚠️ Nota: Se intentó el uso de Unsloth, pero se presentaron múltiples errores de dependencias, por lo que se optó por LlamaFactory.

### 3. Interfaz y pruebas

Puedes probar el modelo directamente desde este Colab:

🔗 [Google Colab de prueba](https://colab.research.google.com/drive/1VYT5Z3XoP_tWISqcpXu2a-UC2S3uNC5e?usp=sharing)

### 4. Generación de imágenes

Las respuestas del chatbot pueden complementarse con imágenes generadas dinámicamente usando **Stable Diffusion XL**.

🔗 [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)

### 5. RAG (Retrieval-Augmented Generation)

Para enriquecer las respuestas con datos más precisos y contextuales, se implementó un sistema RAG con **ChromaDB** como vector store.

---

## 🧠 Detector de Intención y Gemini

El chatbot analiza la intención del usuario y adapta su respuesta. Utiliza **Gemini** para:

- 🧠 Detectar intenciones complejas
- ⚔️ Simular batallas de forma más narrativa y creativa
- ❓ Apoyar el razonamiento en contextos ambiguos

Para preguntas educativas y respuestas informativas se utiliza el modelo fine-tuneado (`Qwen2.5-3B-Instruct` + fine-tuning).

---

## 💡 Funcionalidades Principales

- 🖼️ **Generar imágenes** de animales prehistóricos descritos por el usuario  
- ⚔️ **Simular batallas** entre criaturas (por ejemplo, “¿Quién ganaría entre un T-Rex y un Spinosaurus?”) usando Gemini  
- ❓ **Responder preguntas educativas** sobre historia natural, paleontología y más usando el modelo fine-tuneado  
- 🧠 **Detectar la intención** del usuario y redirigir la respuesta al módulo adecuado  

---

## 🎥 Demostración en Video

📺 [YouTube: Demostración](https://youtu.be/_e8RLyzdNaM)

[![YouTube: Demostración](https://img.youtube.com/vi/_e8RLyzdNaM/0.jpg)](https://youtu.be/_e8RLyzdNaM)

---

## ✨ Proyecto

🔗 [Abrir proyecto en Colab](https://colab.research.google.com/drive/1DGAuAqdxq3iqYEw1JCh0aSR2iImDxj2Y?usp=sharing)
