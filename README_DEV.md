# Entorno de desarrollo

## Opción 1: uv (recomendado)
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
cd DL-QPI
uv sync
```

## Opción 2: venv + pip
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Opción 3: conda
```bash
conda create -n dl-qpi python=3.10
conda activate dl-qpi
pip install -r requirements.txt
```

## Jupyter
```bash
python -m ipykernel install --user --name=dl-qpi --display-name "Python (dl-qpi)"
jupyter lab
```

## Verificar
```bash
python -c "import numpy, pandas, matplotlib, PIL, cv2, skimage, sklearn, torch; print('OK')"
```
