# Sistemas de Decisión Inteligente Basados en Aprendizaje por Refuerzo 🤖

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![AI](https://img.shields.io/badge/Artificial%20Intelligence-Reinforcement%20Learning-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📖 Descripción

Este proyecto desarrolla e implementa diferentes sistemas de toma de decisiones utilizando técnicas de **Aprendizaje por Refuerzo (Reinforcement Learning)**, específicamente el algoritmo **Q-Learning**. Se modelan y resuelven diversos problemas reales mediante agentes inteligentes capaces de aprender políticas óptimas a partir de la interacción con su entorno.

El trabajo fue desarrollado como parte del curso de **Inteligencia Artificial** de la **Universidad Nacional Mayor de San Marcos (UNMSM)**.

---

## 🎯 Objetivos

* Comprender los fundamentos teóricos y prácticos del Aprendizaje por Refuerzo.
* Implementar el algoritmo Q-Learning desde cero sin depender de librerías de RL de alto nivel.
* Modelar problemas de la vida real como Procesos de Decisión de Markov (MDP).
* Analizar el comportamiento de un agente inteligente en distintos escenarios bajo incertidumbre.
* Evaluar el desempeño del aprendizaje mediante simulaciones, gráficos y métricas de convergencia.

---

## 🔍 Casos de Estudio

El proyecto aborda los siguientes escenarios aplicando Q-Learning:

### 📦 Gestión de Inventarios
Optimización de las decisiones de reabastecimiento para minimizar costos de almacenamiento y evitar escenarios de desabastecimiento en la cadena de suministro.

### 🚗 Navegación Autónoma en un Almacén
Diseño de un agente inteligente capaz de encontrar rutas eficientes, evitando obstáculos dinámicos y fijos, y minimizando el tiempo total de recorrido.

### 🛵 Ruteo Óptimo de Delivery con Congestión Variable
Selección de rutas de entrega considerando cambios dinámicos en las condiciones del tráfico y la congestión urbana para optimizar los tiempos de llegada.

### 🏭 Mantenimiento Preventivo Industrial
Aprendizaje de políticas de mantenimiento predictivo que permitan reducir costos operativos, maximizar la vida útil de los equipos y prevenir fallas catastróficas.

---

## 🧠 Algoritmo Implementado

Se emplea el algoritmo **Q-Learning**, una técnica de Aprendizaje por Refuerzo libre de modelo (model-free) y basada en valores, que actualiza iterativamente la función Q utilizando la Ecuación de Bellman:

```math
Q(s,a) \leftarrow Q(s,a) + \alpha \left[ r + \gamma \max_{a'}Q(s',a') - Q(s,a) \right]
```

Donde:
* **s** : Estado actual.
* **a** : Acción ejecutada.
* **r** : Recompensa obtenida por ejecutar la acción $a$ en el estado $s$.
* **α** : Tasa de aprendizaje (Learning Rate) - Determina qué tanto la nueva información sobrescribe a la antigua.
* **γ** : Factor de descuento (Discount Factor) - Determina la importancia de las recompensas futuras.

---

## 🛠️ Tecnologías Utilizadas

* **Lenguaje principal:** Python 3
* **Entorno de desarrollo:** Jupyter Notebook / JupyterLab
* **Cómputo científico y datos:** NumPy, Pandas
* **Visualización:** Matplotlib, Seaborn
* **Teoría de grafos:** NetworkX
* **Interfaces interactivas:** Streamlit

---

## 📂 Estructura del Proyecto

```text
├── Trabajo_Computacional_IA_Aprendizaje_Reforzado.ipynb # Notebook principal con toda la implementación
├── README.md                                            # Documentación del proyecto
├── requirements.txt                                     # Dependencias y librerías necesarias
└── .gitignore                                           # Archivos ignorados por Git
```

---

## 🚀 Instalación y Uso

### 1. Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/nombre-del-repositorio.git
cd nombre-del-repositorio
```

### 2. Instalar las dependencias

Se recomienda el uso de entornos virtuales (`venv` o `conda`). Para instalar las dependencias, ejecuta:

```bash
pip install -r requirements.txt
```

*(Opcional) Si prefieres instalarlo manualmente:*
```bash
pip install numpy pandas matplotlib networkx streamlit jupyter jupyterlab
```

### 3. Ejecutar el Notebook

Inicia el servidor de Jupyter para explorar los casos de estudio:

```bash
jupyter notebook
```
*(O alternativamente, `jupyter lab`)*

---

## 📊 Resultados

Los experimentos realizados a lo largo del notebook demuestran que el algoritmo Q-Learning es capaz de:

* Aprender políticas de decisión eficientes y cercanas al óptimo teórico.
* Adaptarse a diferentes entornos y ajustarse ante variaciones en la función de recompensa.
* Mejorar progresivamente su desempeño a medida que aumentan los episodios de entrenamiento, logrando la convergencia de la Tabla Q.
* Resolver problemas complejos de optimización en contextos de logística, industria y gestión de recursos con alta escalabilidad.

---

## 🏅 Competencias Demostradas

* Inteligencia Artificial
* Aprendizaje por Refuerzo (Reinforcement Learning)
* Algoritmo Q-Learning
* Procesos de Decisión de Markov (MDP)
* Simulación y Modelado de Entornos
* Optimización Heurística
* Análisis Exploratorio de Datos
* Programación Avanzada en Python

---

## 👥 Autores

| Nombre                                | Código   |
| ------------------------------------- | -------- |
| López Salinas, Leonardo Miguel        | 23200104 |
| Tarqui Soncco, Nicolás Alejandro Inti | 23200121 |
| Cueva Alcala, Axel Andree             | 23200093 |
| Carrasco Flores, Ángel Giovanny       | 23200086 |

**Universidad Nacional Mayor de San Marcos**  
Facultad de Ingeniería de Sistemas e Informática (FISI)  
Curso: Inteligencia Artificial  

---

## 📄 Licencia

Este proyecto fue desarrollado con fines académicos y educativos para el curso de Inteligencia Artificial de la UNMSM.