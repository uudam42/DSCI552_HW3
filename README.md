# DSCI 552 Homework 3

Time series feature extraction on the UCI Activity Recognition (AReM) data set, plus ISLR exercise 3.7.4.

## Structure

```
.
├── data/
│   ├── AReM/
│   │   ├── bending1/ ... walking/      # 7 activity folders, 88 instances
│   │   ├── bendingType.pdf
│   │   └── sensorsPlacement.pdf
│   └── arem_features.csv               # 42 extracted features (written by the notebook)
├── notebook/
│   └── Agudanmu_Danmu_HW3.ipynb
└── requirements.txt
```

## How to run

```bash
pip install -r requirements.txt
cd notebook
jupyter notebook Agudanmu_Danmu_HW3.ipynb
```

The notebook reads the data with the relative path `../data/AReM/`, so it should be run from the `notebook/` folder. The raw files need minor cleaning (comment header lines, one space-separated file, trailing commas), which is handled by the loader in the notebook, so the original files are used unchanged.

The extracted features are saved to `data/arem_features.csv` so they can be reused in Homework 4.
