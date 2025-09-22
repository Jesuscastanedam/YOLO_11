# YOLO 11 Object Detection Explorer

## Descripción

Este proyecto utiliza YOLO 11, el último modelo de detección de objetos de Ultralytics, para realizar reconocimiento en tiempo real a través de la webcam. El código está adaptado del trabajo de **Albert Coronado Calzada**.

## Características

- Detección de objetos en tiempo real usando YOLO 11
- Interfaz de webcam integrada
- Visualización de cajas delimitadoras con etiquetas de confianza
- Soporte para más de 80 clases de objetos (dataset COCO)

## Configuración del Entorno

### 1. Crear entorno virtual

```bash
# Crear entorno virtual
virtualenv venv 

# Activar entorno virtual
# Linux/Mac:
source venv/bin/activate

# Windows:
venv\Scripts\activate
```

### 2. Instalar dependencias

```bash
pip install -r requirements.txt
```

Las principales dependencias incluyen:
- ultralytics
- opencv-python
- torch

### Controles

- **'q'**: Presiona para salir de la aplicación

## Funcionalidad

El sistema:

1. Carga el modelo YOLO 11 preentrenado (`yolo11l.pt`)
2. Captura video en tiempo real desde tu webcam
3. Procesa cada frame para detectar objetos
4. Dibuja cajas delimitadoras alrededor de los objetos detectados
5. Muestra el nombre del objeto y su nivel de confianza

## Resultados Experimentales

Durante las pruebas, el modelo demostró:

**Detecciones exitosas:**
- Personas
- Dispositivos móviles (iPhone)
- Botellas de agua

**Limitaciones observadas:**
- Confusión entre objetos pequeños (ej: figura de Luigi detectada como tarta)

Esto ilustra tanto el potencial como las limitaciones actuales de los sistemas de visión por computadora, que dependen de los datos de entrenamiento del modelo.

## Estructura del Proyecto

```
.
├── Explorer.ipynb          # Notebook principal con análisis paso a paso
├── requirements.txt        # Dependencias del proyecto
└── README.md               # Este archivo
```

## Modelo YOLO 11

YOLO 11 representa el estado del arte en detección de objetos, ofreciendo:
- Mayor precisión que versiones anteriores
- Procesamiento en tiempo real optimizado
- Soporte para múltiples tareas de visión por computadora

## Créditos

Código adaptado del trabajo de **Albert Coronado Calzada**.

Basado en el modelo YOLO 11 de [Ultralytics](https://docs.ultralytics.com/models/yolo11/).

## Aplicaciones Potenciales

Este tipo de tecnología tiene aplicaciones infinitas:
- Sistemas de seguridad inteligentes
- Aplicaciones en retail y manufactura
- Análisis de comportamiento
- Robótica y vehículos autónomos
- Aplicaciones médicas y de salud

## Licencia

Este proyecto es de propósito educativo y experimental.
