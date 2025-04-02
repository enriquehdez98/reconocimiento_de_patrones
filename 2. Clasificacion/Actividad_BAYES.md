# **Actividad: Implementando un Clasificador Bayesiano desde Cero**

## **Objetivo:**
Escribir un programa en Python que implemente el clasificador **Naïve Bayes** desde cero, sin usar librerías como `scikit-learn`, solo `pandas` para manejar los datos.

---
## **Actividad:**
- Constesta el siguiente formulario: https://forms.office.com/r/Q6iG19kEeL
- Utiliza el código del clasificador para predecir qué personas son **usuarios premium en Spotify**.

---
## **Filtrar datos con Pandas**

### **Ejemplo 1: Filtrar en pandas con dos condiciones (AND)**

Supongamos que tenemos un DataFrame con información sobre productos y queremos filtrar solo aquellos que sean **"Rojo" y de "Tamaño Grande"**.

```python
import pandas as pd

# Crear un DataFrame de ejemplo
data = pd.DataFrame({
    "Color": ["Rojo", "Azul", "Rojo", "Verde", "Azul", "Rojo"],
    "Tamaño": ["Grande", "Pequeño", "Mediano", "Grande", "Mediano", "Pequeño"],
    "Precio": [10, 15, 20, 10, 30, 25]
})

# Filtrar donde Color sea "Rojo" y Tamaño sea "Grande"
filtro = (data["Color"] == "Rojo") & (data["Tamaño"] == "Grande")
data_filtrada = data[filtro]

print(data_filtrada)
```

---

Este código muestra cómo filtrar datos en **pandas** usando condiciones múltiples con `&` (**AND**).

Para aplicar este concepto al **clasificador bayesiano**, puedes adaptar los filtros para trabajar con datos de usuarios de **Spotify** y predecir si son **usuarios premium**. 🚀

