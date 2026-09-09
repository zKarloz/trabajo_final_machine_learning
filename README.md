# Predicción de acciones de Microsoft

Proyecto de Trbajo Final de Machine Learning que analiza el historial de las acciones de Microsoft y clasifica si el cierre de la siguiente jornada subirá o no. También incluye un análisis NLP del reporte anual 2021 de Microsoft.

## Archivos necesarios

Coloca en una misma carpeta:

- `Microsoft_Machine_Learning_V2.ipynb`
- `MSFT.csv`
- `Microsoft_AR2021.html` *(opcional, para ejecutar NLP sin internet)*

## Crear y activar el entorno virtual

```bash
python -m venv .venv
```

En PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

En Git Bash:

```bash
source .venv/Scripts/activate
```

## Instalar las librerías

```bash
python -m pip install --upgrade pip
python -m pip install numpy pandas matplotlib seaborn scikit-learn
python -m pip install jupyter ipykernel nltk scipy beautifulsoup4
python -m pip install torch
```

Si la instalación de PyTorch falla, utiliza el comando recomendado para tu sistema en <https://pytorch.org/get-started/locally/>.

## Ejecutar el proyecto

1. Abre el notebook en VS Code o Jupyter.
2. Selecciona como kernel el entorno `.venv`.
3. Comprueba que el CSV se encuentre junto al notebook.
4. Ejecuta las celdas en orden.

El bloque NLP busca primero `Microsoft_AR2021.html`. Si no encuentra el archivo, intenta consultar el reporte oficial por internet.

## Librerías principales

| Librería | Uso en el proyecto |
|---|---|
| Pandas y NumPy | Preparación y transformación de datos |
| Matplotlib y Seaborn | Gráficos |
| Scikit-learn | Random Forest, escalado y métricas |
| PyTorch | Red neuronal |
| NLTK | Tokenización y conteo de palabras |
| SciPy | Matriz dispersa y similitud del texto |
| BeautifulSoup | Extracción de párrafos del reporte anual |

Este proyecto tiene fines educativos. Sus predicciones no garantizan resultados de inversión.
