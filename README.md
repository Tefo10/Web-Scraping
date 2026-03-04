# Web Scraping FBRef

Scraper de FBRef (La Liga) con limpieza de datos y exportacion a CSV.

## Fuente publica
- https://fbref.com/en/comps/12/schedule/La-Liga-Scores-and-Fixtures

## Archivos principales
- `run_scraper.py`: ejecuta el scraping y guarda CSV.
- `src/scraper/stealth_driver.py`: extraccion, limpieza y transformacion de datos.
- `requirements.txt`: dependencias minimas para scraping.

## Ejecucion local
```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python -m playwright install chromium
python run_scraper.py
```

## Salida esperada
- `data/la_liga_stats.csv`
