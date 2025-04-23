# 🧠 Corrección de errores usando Hamming (7,4)

**Autor**: Mg. Ing. Martin Karlo Verastegui Ponce  
**Versión**: 1.0  
**Lenguaje**: Python 3  
**Propósito**: Educación, demostración y simulación de sistemas de comunicación confiables

---

## 1. 🎯 Descripción del Proyecto

Este script simula un sistema de transmisión de datos binarios utilizando el **Código Hamming (7,4)**, uno de los métodos más conocidos para la detección y corrección de errores de un solo bit.

🔐 **Características principales:**

- ✅ **Codificar:** Mensaje de 4 bits con 3 bits de paridad.  
- ⚠️ **Simular errores:** Introducir fallos intencionales en la transmisión.  
- 🛠️ **Detectar y corregir:** Automatizar la corrección de un solo bit dañado.  
- 🔍 **Decodificar y verificar:** Asegurar la integridad de los datos originales.  

> Ideal para estudiantes y profesionales en **telecomunicaciones**, **sistemas digitales**, **sistemas embebidos** y **educación tecnológica**.

---

## 2. 📦 ¿Qué hace el script?

1. **Entrada:** Solicita al usuario 4 bits de datos.  
2. **Codificación:** Genera un mensaje de 7 bits (4 datos + 3 paridad).  
3. **Error simulado:** Invierte un bit para demostrar la detección.  
4. **Detección:** Calcula el síndrome binario para localizar el error.  
5. **Corrección:** Corrige automáticamente el bit erróneo.  
6. **Decodificación:** Extrae y muestra los 4 bits originales.  
7. **Verificación:** Compara y confirma si la recuperación fue exitosa.  

---

## 3. 🧰 Requisitos

- **Python 3.7** o superior  
- **Sin librerías externas**  
- Ejecución desde **terminal** o **consola interactiva**  

---

## 4. 🚀 Cómo ejecutar

1. Clona este repositorio o copia el archivo `hamming_74.py`:
   ```bash
   git clone https://github.com/tu_usuario/hamming-hamming74.git
   cd hamming-hamming74
   ```
2. Ejecuta el script:
   ```bash
   python hamming_74.py
   ```
3. Ingresa tus datos cuando se te pida:
   ```
   Ingrese 4 bits separados por espacio (ej: 1 0 1 1): 1 0 0 1
   ```

---

## 5. 🧪 Ejemplo de salida

```console
🧠 Corrección de errores Hamming (7,4) v1.0
👨‍🏫 Autor: Mg. Ing. Martin Karlo Verastegui Ponce

Ingrese 4 bits separados por espacio (ej: 1 0 1 1): 1 0 0 1

📦 Codificando los datos...
✅ Datos codificados (7 bits): [0, 1, 1, 0, 0, 1, 1]

⚠️ Se ha introducido un error en la posición 4: [0, 1, 1, 1, 0, 1, 1]

🛠️ Error detectado en la posición 4. Bit corregido.
📨 Mensaje corregido: [0, 1, 1, 0, 0, 1, 1]

🔍 Datos decodificados: [1, 0, 0, 1]
🎉 ¡Éxito! Los datos fueron recuperados correctamente.
```

---

## 6. 📚 Fundamento teórico

El **Código Hamming (7,4)**, propuesto por Richard W. Hamming, permite:

- Detectar hasta **2 errores**.  
- Corregir **1 error**.  
- Utilizar 3 bits de paridad (en posiciones de potencias de 2) para proteger 4 bits de datos.

Se emplea comúnmente en memorias RAM, sistemas de comunicación, discos ópticos y entornos donde la confiabilidad es crítica.

---

## 7. 📌 Estructura del mensaje Hamming

| Posición | Contenido     |
|----------|---------------|
| 1        | p1 (paridad)  |
| 2        | p2 (paridad)  |
| 3        | d1 (dato)     |
| 4        | p3 (paridad)  |
| 5        | d2 (dato)     |
| 6        | d3 (dato)     |
| 7        | d4 (dato)     |

Los bits de paridad cubren posiciones específicas, permitiendo el cálculo de un **síndrome binario** que indica la posición exacta del error.

---

## 8. 💡 Posibles mejoras

- Interfaz gráfica con **Tkinter** o **PyQt**.  
- Versión web usando **Flask** o **Streamlit**.  
- Visualización interactiva de errores y correcciones.  
- Soporte para códigos avanzados: **BCH**, **Reed-Solomon**, etc.

---

## 9. 👨‍🏫 Autor

**Mg. Ing. Martin Karlo Verastegui Ponce**  
Docente y especialista en IA, control automático, teleoperación y educación tecnológica aplicada.

---

## 10. 📄 Licencia

Proyecto distribuido bajo **Licencia MIT**.  
Uso, modificación y distribución permitidos con fines académicos y personales. 🙌
