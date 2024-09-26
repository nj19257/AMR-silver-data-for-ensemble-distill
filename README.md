# AMR Silver Data for Ensemble Distillation

This repository contains details and instructions for accessing a high-quality silver dataset for Abstract Meaning Representation (AMR) parsing, consisting of 362,000 sentence-AMR pairs. The dataset is created through an ensemble distillation process, combining multiple AMR parsers to produce reliable AMR annotations for robust model training.

## About the Dataset
The silver dataset was generated using the Maximum Bayes Smatch Ensemble Distillation (MBSE) technique, which leverages outputs from different pre-trained AMR parsers. The dataset aims to provide extensive linguistic diversity and varied sentence structures, contributing to the development of advanced AMR parsing models.

### Key Features
- **362,000 Sentence-AMR Pairs**: Making it one of the largest silver datasets for AMR parsing.
- **Enhanced Model Performance**: The increased size of the training corpus has shown a positive impact on the performance of the student model, resulting in higher Smatch scores.
- **Diverse Annotations**: Uses multiple models with different seed releases for a comprehensive set of AMR graphs.

## Maximum Bayes Smatch Ensemble Distillation (MBSE)
The **MBSE** method is a Smatch-based ensembling technique that generates high-quality AMR annotations by combining the outputs of multiple teacher models. This ensemble output is used as distillation knowledge for training a student model.

### Methodology
- **Trained Parsers**:  
  We employed three instances of the **AMR3-structbart-Large** model, each trained on the gold-labeled **AMR 3.0** dataset with different seed releases from IBM Research. This model leverages action sequences, which produce more accurate AMR graphs with reduced noise.
- **Parsing Unlabeled Text**:  
  The trained parsers were used to annotate unlabelled English text, resulting in diverse samples of AMR parses.
- **Smatch-Based Ensemble Algorithms**:  
  Multiple Smatch-based algorithms, including **Graphene-Smatch**, **Greedy-Select**, and **Average-Smatch**, were tested to integrate outputs from the parsers. **Average-Smatch** was selected for its simplicity and competitive performance.

## Download the Dataset
The silver AMR dataset is available for download from Google Drive. Due to the size constraints of GitHub, the dataset is hosted externally. 

📦 [Download the Final Ensembled Silver AMR Dataset (362,000 sentence-AMR pairs)](https://drive.google.com/file/d/1tDmZwRZj9h81guDO0meZZQq5PRf00L0B/view?usp=sharing)

Alternatively, the dataset can be accessed in the silver dataset from the three IBM_Research amr parsers before applying the ensemble method from [this link](https://drive.google.com/drive/folders/1qdNhJQQ9VEljP-Asz43iqfDre9rKxbFv?usp=sharing).

## Usage and License
This dataset is open for research and non-commercial use to aid in the advancement of AMR parsing techniques. If you use this dataset in your work, please consider citing the original sources, as well as the papers related to the MBSE methodology and AMR parsing models.

### Citation
When using this dataset, please cite the original works:

- **GLUE Benchmark**: 
- **CoLA**: 
- **MRPC**: 
- **QNLI**: 
- **XSum Dataset**: 
- **AMR3-structbart-Large Model**: 
- **Maximum Bayes Smatch Ensemble Distillation**: 

## Contact
For questions, suggestions, or collaboration opportunities, please reach out through issues

Happy parsing! 🚀
