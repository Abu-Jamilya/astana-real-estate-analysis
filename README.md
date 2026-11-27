# Astana apartment asking prices

This is our group final project for **LING 231 — Programming for the Humanities & Social Sciences** at **Nazarbayev University**. We use Python to ask how advertised apartment prices in Astana vary with floor area, room count, district, building material, construction year, and floor.

## Explore the project

| File | What it contains |
| --- | --- |
| [data_analysis.ipynb](data_analysis.ipynb) | The main notebook, with the team's calculations and eight saved plots. |
| [astana_apartments.csv](astana_apartments.csv) | A snapshot of 932 Krisha.kz advertisements with 13 fields, including price in tenge, area in m², listing URL, and building characteristics. |
| [data_parsing.ipynb](data_parsing.ipynb) | The collection notebook, showing how listing cards were read and exported to CSV. |

## What did the listings show?

The median asking price was **40,027,400 KZT** across the 932 advertisements. Dividing each asking price by its floor area and averaging those values gives **678,396 KZT/m²**. The district comparison ranged from **512,711 KZT/m² in Baikonur** to **744,338 KZT/m² in Esil** among listings matched to the six district labels in the notebook.

These figures describe asking prices in this sample. Of the 932 advertisements, **196 quote a starting price** (`price_from = 1`). The notebook includes those advertised amounts in its summaries. Sale prices and the final amount paid by a buyer are unknown.

## Run the analysis

1. Download [astana_apartments.csv](https://raw.githubusercontent.com/Abu-Jamilya/astana-real-estate-analysis/main/astana_apartments.csv) and keep that filename.
2. [Open the analysis notebook in Google Colab](https://colab.research.google.com/github/Abu-Jamilya/astana-real-estate-analysis/blob/main/data_analysis.ipynb). In the **Files** sidebar, upload the CSV to the default working directory.
3. Choose **Runtime → Run all**. To run locally, open the notebook in Jupyter with Python 3 and Matplotlib installed, and keep the CSV beside the notebook.

The analysis uses the included snapshot. The collection notebook's saved output shows an interrupted run after HTTP 403 responses, and its saved export message reports 43 rows. To experiment with collection, run it in a separate working directory because its export cell writes a file named `astana_apartments.csv`.

Codex helped prepare this README and adapt the analysis notebook to load the included CSV.
