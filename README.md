# Chatbot PDF Inteligente con FLAN-T5

---

## 1. INSTALAR LIBRERÍAS
<img width="1057" height="87" alt="image" src="https://github.com/user-attachments/assets/09614171-3999-4461-b9ee-408315fe32c8" />

### ¿Qué hace?
Instala las librerías necesarias para ejecutar el proyecto.

### Librerías utilizadas:
- gradio → Interfaz web (chatbot)  
- transformers → Modelos de IA  
- sentence-transformers → Embeddings (vectores)  
- faiss-cpu → Búsqueda de similitud  
- pypdf → Lectura de PDFs  
- accelerate → Optimización  

---

## 2. IMPORTAR LIBRERÍAS
<img width="690" height="217" alt="image" src="https://github.com/user-attachments/assets/133943e3-3935-4309-9977-d8dc225e538e" />

### ¿Qué hace?
Carga todas las herramientas necesarias para el funcionamiento del programa.

---

## 3. VARIABLES GLOBALES
<img width="512" height="72" alt="image" src="https://github.com/user-attachments/assets/1dc532af-9614-41a8-a1e4-c0f466232e3d" />

- documents → Almacena fragmentos de texto  
- index → Estructura de búsqueda  

### Modelos utilizados:
<img width="572" height="52" alt="image" src="https://github.com/user-attachments/assets/3d92a739-dd34-47ce-9811-a3a9a9ebaf66" />

- Modelo de embeddings: Convierte texto en vectores numéricos

  <img width="857" height="73" alt="image" src="https://github.com/user-attachments/assets/727d81b9-291f-43e8-a5fd-a98398e656a4" />

- Modelo FLAN-T5:
  - Tokenizer → Convierte texto a números  
  - Modelo → Genera respuestas inteligentes  

---

## 4. FUNCIÓN: LEER PDF

<img width="562" height="522" alt="image" src="https://github.com/user-attachments/assets/dd21e56d-04be-45a1-9395-17860bda39e9" />

### ¿Qué hace?
- Lee el archivo PDF  
- Extrae el texto  
- Limpia saltos de línea y espacios  

---

## 5. FUNCIÓN: CARGAR PDFs
<img width="753" height="652" alt="image" src="https://github.com/user-attachments/assets/c43c29e9-80e8-46f2-a742-91ae54aac638" />

### ¿Qué hace?
- Lee los PDFs  
- Divide el texto en fragmentos (chunks)  
- Convierte cada fragmento en vectores  
- Los guarda en FAISS para búsquedas rápidas  

---

## 6. FUNCIÓN: BUSCAR CONTEXTO
<img width="766" height="338" alt="image" src="https://github.com/user-attachments/assets/cfa0e24d-f8c9-4a56-b24a-1e311d15208c" />

### ¿Qué hace?
- Convierte la pregunta en vector  
- Busca los textos más similares  
- Devuelve el contexto relevante  

---

## 7. FUNCIÓN: CHATBOT
<img width="1007" height="677" alt="image" src="https://github.com/user-attachments/assets/3ecf3bd5-cfa8-417d-9c5c-0d6ca09de426" />
<img width="867" height="257" alt="image" src="https://github.com/user-attachments/assets/07684cbe-9f39-49ea-9a67-46337181e1f8" />

### ¿Qué hace?
- Recibe la pregunta del usuario  
- Busca contexto relevante  
- Genera una respuesta con IA  
- Actualiza el historial del chat  

---

## 8. INTERFAZ (GRADIO)
<img width="817" height="723" alt="image" src="https://github.com/user-attachments/assets/4f18334d-0b7d-45bd-8fed-edcf41dfc2da" />
<img width="807" height="391" alt="image" src="https://github.com/user-attachments/assets/893f50be-88e7-4d70-8fc5-2b5d825ab3de" />

### ¿Qué hace?
- Crea la interfaz web  
- Permite subir archivos PDF  
- Permite hacer preguntas al chatbot  

---

## 9. EJECUTAR APLICACIÓN

<img width="1693" height="636" alt="image" src="https://github.com/user-attachments/assets/f511c1b4-34d1-4260-a4cf-c3f9fb3eaec7" />

### ¿Qué hace?
- Inicia el chatbot  
- Genera un enlace público para acceder  

---

## RESULTADO FINAL

Este proyecto permite:


<img width="792" height="478" alt="image" src="https://github.com/user-attachments/assets/699bee07-5020-43a2-8614-781eaf2b2dd7" />
<img width="803" height="217" alt="image" src="https://github.com/user-attachments/assets/f335358a-5f80-48e4-9ab1-b7d5cde69a86" />

<img width="791" height="500" alt="image" src="https://github.com/user-attachments/assets/fa2f51c8-454c-4301-ae02-a638725b39ed" />

- Subir múltiples PDFs  
- Buscar información relevante automáticamente  
- Generar respuestas inteligentes en español  
- Interactuar mediante una interfaz web  
