# Descarga-Imagenes-Astronomicas


---

# 🌌 Descarga de Imágenes Astronómicas  

### 📷 Proyecto para la obtención de imágenes astronómicas a partir de coordenadas celestes  

Este proyecto permite **descargar imágenes astronómicas** utilizando coordenadas celestes.  
Utiliza el servicio en línea del **Sloan Digital Sky Survey (SDSS)** para obtener imágenes de galaxias y otros objetos astronómicos a partir de sus coordenadas de **Ascensión Recta (RA) y Declinación (DEC)**.  

---

## 🚀 **Características**
✅ Descarga imágenes del **SDSS** automáticamente a partir de coordenadas.   
✅ Guarda las imágenes en una carpeta estructurada.  
✅ Posibilidad de convertir imágenes a **arrays NumPy** para su análisis (opcional).  
✅ Soporte para la carga de datos desde archivos CSV.  

---

## 📂 **Estructura del Proyecto**

📁 DESCARGA IMÁGENES ASTRONÓMICAS  
│── 📂 001.DATOS/                # Archivos de coordenadas y datos adicionales  
│── 📂 001.IMAGENES DESCARGADAS/  # Carpeta donde se almacenan las imágenes descargadas  
│── 📝 Trabajo Imágenes.ipynb     # Notebook principal con la implementación del código  
│── 📄 README.md                  # Este archivo con la documentación  


---

## 🔧 **Instalación y Configuración**  
Para ejecutar el código, primero instala las dependencias necesarias (disponible directamente en el notebook):  

```sh
pip install numpy pandas matplotlib seaborn h5py requests tqdm pillow
```

Luego, clona el repositorio y accede a la carpeta:  

```sh
git clone https://github.com/RaulDiezRiesco/Descarga-Imagenes-Astronomicas.git
cd Descarga-Imagenes-Astronomicas
```

---

## 🔍 **Uso del Proyecto**  
### 1️⃣ **Cargar los Datos de Coordenadas**
El programa lee un archivo CSV con coordenadas astronómicas como ejemplo:  

### 2️⃣ **Generar URLs para Descargar Imágenes**
El código genera URLs del SDSS a partir de coordenadas en J2000:  

### 3️⃣ **Descargar las Imágenes**
Se itera sobre las coordenadas y se descargan las imágenes en la carpeta **"001.IMAGENES DESCARGADAS"**.  

### 4️⃣ **Visualización de Imágenes**
Para visualizar una imagen específica desde el DataFrame:  

## 📌 **Notas Importantes**
- Si el número de imágenes es **muy alto**, cargarlas en memoria puede ser costoso para el ordenador.  
  - Se recomienda **reducir la resolución** o **cargar imágenes solo cuando sean necesarias**.  
- Si alguna imagen **no se encuentra en SDSS**, el código manejará el error sin detener la ejecución.  
- Se puede modificar la URL para obtener imágenes de **otras bases de datos astronómicas** como DSS o Pan-STARRS.  

---

## 🔄 **Actualización del Proyecto**
Si realizas cambios en el código, sube las modificaciones a GitHub con:  

```sh
git add .
git commit -m "Descripción del cambio"
git push origin main
```

Si necesitas actualizar tu repositorio local con los últimos cambios en GitHub:  

```sh
git pull origin main
```

---
