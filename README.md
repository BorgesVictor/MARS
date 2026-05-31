**MARS (Meta-learning for Anonymization Recommendation and Selection)** is a meta-learning framework designed to automate the selection of anonymization techniques based on dataset characteristics.

The framework addresses a fundamental challenge in privacy-preserving data publishing: selecting the most appropriate anonymization technique while maintaining a balance between privacy protection and data utility. Instead of relying on manual trial-and-error procedures, MARS learns from previous anonymization scenarios and recommends the technique that is expected to provide the best utility for a given dataset.

To build the recommendation model, multiple anonymization techniques, including **k-anonymity**, **l-diversity**, **t-closeness**, and **differential privacy**, are applied to a collection of tabular datasets. The resulting anonymized datasets are evaluated using machine learning models, and dataset characteristics are extracted through meta-features. These meta-features are then used to train meta-models capable of predicting the most suitable anonymization technique for unseen datasets.

This repository contains all artifacts associated with the MARS framework, including datasets, anonymized datasets, extracted meta-features, source code, experimental results, and supplementary materials required to reproduce the study.

## Repository Structure

### `codigos`

Source code and notebooks used to conduct the experiments and generate the results reported in the study.

### `dados`

Original datasets used throughout the experimental evaluation.

### `dados_originais_anonimizados`

Anonymized versions of the original datasets generated using the evaluated privacy-preserving techniques.

### `dados_originais_anonimizados_codificados`

Encoded versions of the anonymized datasets prepared for machine learning and meta-learning tasks.

### `dados_bagging_anonimizados`

Bootstrap and bagging-based anonymized datasets used during the experimental procedures.

### `Meta_features`

Extracted meta-features describing the characteristics of the datasets used in the meta-learning stage.

### `Target_Meta_Modelo`

Target variables and outputs employed for training and evaluating the meta-models.

### `resultados_metricas`

Performance metrics and experimental results obtained throughout the study.

### `Premissas`

Experimental assumptions, configurations, and supporting files used during the research.

## Reproducibility

All files required to reproduce the experiments reported in the article are provided in this repository, including datasets, anonymized datasets, extracted meta-features, source code, and evaluation results.

## Citation

If you use this repository in your research, please cite the associated publication.

## License

This repository is intended for academic and research purposes.
