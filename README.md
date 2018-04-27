# Sistema para la automatización en el analisis de contratos para CNBV
## Autor: Juan Salvador Cortés Francisco
---
### Problema
La nececidad de extraer información de los contratos en la CNBV para poder cumplir con la Ley de Trasparencia **__Editar con la ley__** y la cantidad de contratos que se necesitan procesar.

### Tecnologias

### Pre-procesamiento
*   De 'color' a blanco y negro
    *   Filtros de enfoque
    *   Quitar el resaltado a regiones con color
    *   Umbral adaptativo
*   Recortar la imagen
    *   Retirar areas innecesarias
*   Extraer las lineas
    *   Reconocimiento de lineas (Constraint algorithm)

### Procesamiento
*   Tesseract
    *   Datos para entrenar

### Extracción de datos estructurados
*   Analizador
    *   Entrada: Texto
    *   Salida: Documento estructurado
*   Elementos a extraer
    *   Número de contrato
    *   Tipo de procedimiento
    *   **Completar**
*   Distancia de Levenshtein

### Requisitos
```
brew cask install xquartz
brew install poppler antiword unrtf tesseract swig
pip install textract
```

