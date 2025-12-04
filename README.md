# GeoFM-Romania-SceneClassification

## Geospatial Foundation Models: Scene Classification

This repository hosts the materials for a scene classification project completed as part of the **Passion in Action: Artificial Intelligence for the Earth: Geospatial Foundation Models (PiA-AI4E-GeoFM)** course at Politecnico di Milano.

### Project Goal

The core objective is to investigate the efficacy of modern Geospatial Foundation Models (GFMs) for Earth Observation tasks.

We perform **Land Cover Scene Classification** for a case study over **Romania**. This involves comparing the performance of two prominent GFMs:

1.  **TerraMind:** An advanced, multimodal, and generative GFM.
2.  **Prithvi:** A versatile, multi-temporal representation model.

### Workflow Summary

1.  **Data Generation:** A custom dataset of **at least 100 image chips** over Romania was generated using ground-truth points from the **LUCAS dataset** and Google Earth Engine (GEE).
2.  **Model Fine-Tuning:** Both Prithvi and TerraMind models were fine-tuned for the classification task, utilizing the PyTorch Lightning/TerraTorch framework.
3.  **Evaluation & Comparison:** Model performance metrics (Accuracy, F1-Score, Confusion Matrices) are compared to draw conclusions on their respective suitability for regional land cover analysis.

### Repository Contents

* `lucas_image_chips.ipynb`: Notebook used to query GEE, filter LUCAS points for Romania, and download the raw image chip dataset.
* `finetuning_terramind.ipynb`: The adapted notebook containing the PyTorch Lightning/TerraTorch pipeline for fine-tuning TerraMind on the generated dataset.
* `finetuning_prithvi.ipynb`: The notebook detailing the fine-tuning of the Prithvi model.
* `data/`: Directory (linked to Google Drive) containing the custom `lucas_image_chips.ipynb`, the dataset will be on google drive.
* `report.pdf`: Final PDF report summarizing the methodology, experiments, and comparative results.
