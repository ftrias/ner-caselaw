## Experiments

Compute infrastructure: 
- AMD Ryzen 7 3700X 8-Core
- 32 GB RAM
- NVIDIA 1080Ti GPU

Compute time: 
- HCL-NER trainning: 4 hours, 24 minutes

Libraries: 
- python, pandas, numpy, matplotlib, scipy, seaborn, joblib, fuzzy, flair, nameparser, networkx

Number of parameters: 
- FLERT: 19397142
- PoS: 62243302

Validation perfomance: 
- For HCL-NER for the tag PER (person) 
  - tp: 22940 - fp: 955 - fn: 790
  - precision: 0.9600 - recall: 0.9667
  - f1-score: 0.9634

Metrics used: 
- F1 score
- Accuracy as a percent of text parsed correctly.

## Data

Data source: 
- Harvard Caselaw Access Project
  - English language legal cases from United States since 1700s
  - 40 million pages of text

Manually annotated: 
- 1490 cases total manually annotated for this project by the authors. 
  - 1000 used to train HCL-NER model. 
  - 490 used to compare the accuracy of different methods.

## Files and directories

### Code

| File | Description |
| ---- | ------------|
| abbrev.py      | Library for abbreviations of names. |
| nicknames.py   | Library for nicknames. |
| load_state_nlp.ipynb | Jupyter notebook with parsing and analysis code. |
| train-ner.ipynb | Model training for HCL-NER. |

### Data

| Directory | Description |
| ---- | ------------|
| lang/train/ | 1000 annotated cases for model training. |
| out/ | 490 annotated cases to compare accuracy. |
| images/ |  |
| tables/ |  |
