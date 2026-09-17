# Astronomical Objects Classifier

An earlier iteration of an SDSS-based astronomical-object classification pipeline, focused on data acquisition, preprocessing, and convolutional neural-network experiments.

For the expanded multi-model project—including photometric color-index experiments and stellar spectral classification—see [`AstronomicalObjectsClassifier_new`](https://github.com/GrantDeljevic/AstronomicalObjectsClassifier_new).

## What’s Included

- Sloan Digital Sky Survey (SDSS) data retrieval
- Image and catalog-data preprocessing
- CNN model training and evaluation
- Reusable project structure for datasets, models, notebooks, and logs

## Setup

Python 3.11 is recommended.

```bash
git clone https://github.com/GrantDeljevic/AstronomicalObjectsClassifier.git
cd AstronomicalObjectsClassifier
python -m venv .venv
```

Activate the environment, then install dependencies:

```bash
pip install -r requirements.txt
```

For example, SDSS catalog data can be fetched from the project root with:

```bash
python -m src.data_fetch.fetchCsvSearchTargetData
```

This repository contains research code and assumes the project's original data layout; paths or dataset configuration may need adjustment on a new machine.
