# TAREA-2-PYTHON-
Repositorio dedicado a las tareas iniciales de Python, enfocadas en la generación de números aleatorios, uso de loops y almacenamiento de resultados en disco local, Google Drive y Google Colab. Este proyecto incluye ejemplos de código, instrucciones paso a paso y ejercicios prácticos para reforzar el aprendizaje.
# Tarea 2: Guardar Resultados en Disco Local, Google Drive o Colab

## Propósito de la Actividad
El objetivo de esta actividad es aprender a modificar códigos para guardar resultados generados, como gráficos y datos, en diferentes ubicaciones:
- **Disco local**: Descargar directamente los archivos generados a tu computadora.
- **Google Drive**: Almacenar los resultados en tu unidad de Google Drive para fácil acceso y respaldo.
- **Entorno Colab**: Guardar y descargar resultados directamente desde el cuaderno.

---

## Instrucciones para los Estudiantes

### **Paso 1: Configurar el Entorno de Trabajo**
1. Abre el cuaderno en **Google Colab**.
2. Inicia sesión con tu cuenta de Google para habilitar el acceso a Google Drive si es necesario.

---

### **Paso 2: Guardar en Disco Local**
1. Modifica los bloques de código para guardar gráficos como imágenes en tu computadora.
   - Usa el método `plt.savefig()` antes de `plt.show()` y define un nombre de archivo y formato (PNG, JPG, etc.).

   **Ejemplo:**
   ```python
   import matplotlib.pyplot as plt

   # Generar un gráfico de ejemplo
   plt.plot([1, 2, 3, 4], [10, 20, 25, 30])
   plt.title("Gráfico de Ejemplo")

   # Guardar el gráfico
   plt.savefig("grafico_ejemplo.png")
   plt.show()

   from google.colab import drive
drive.mount('/content/drive')

plt.savefig("/content/drive/My Drive/grafico_ejemplo.png")
plt.show()
with open("resultados_temperaturas.txt", "w") as file:
    file.write("Temperatura promedio: 25.5°C\n")
    file.write("Temperatura máxima: 28°C\n")
    file.write("Temperatura mínima: 23°C\n")

    from google.colab import files
files.download("resultados_temperaturas.txt")
33 IMAGENES DE LA ACTIVIDAD 
![image](https://github.com/user-attachments/assets/82e8c67c-593b-4d90-ad1b-ed475939d842)

![image](https://github.com/user-attachments/assets/8792545b-11c9-49b4-a3b1-25d6be33f858)


## Conclusión
Esta actividad enseña cómo interactuar con sistemas de almacenamiento local y en la nube, como Google Drive, desde Python en Google Colab. Estos conocimientos son esenciales para gestionar y organizar resultados de manera eficiente en entornos de análisis de datos y simulaciones.






