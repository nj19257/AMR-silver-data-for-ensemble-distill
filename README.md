# AMR Silver Data for Ensemble Distillation

This repository hosts the details and instructions for accessing a high-quality silver dataset for Abstract Meaning Representation (AMR) parsing. The dataset has been created by integrating carefully selected subsets from the GLUE benchmark and the EdinburghNLP/XSum dataset, to provide a robust collection of sentences for AMR representation learning.

## About the Dataset
The silver dataset is generated using ensemble distillation techniques with three instances of the AMR3-structbart-Large model, trained on the AMR 3.0 dataset. These models were selected for their ability to produce more accurate AMR graphs with reduced noise, focusing on sentence diversity and high-quality annotation.

### Data Sources
- **GLUE Benchmark**: Subsets included are:
  - **AX**: Manually-curated for linguistic analysis across diverse phenomena.
  - **CoLA (Corpus of Linguistic Acceptability)**: Sentences marked as grammatically acceptable.
  - **MRPC (Microsoft Research Paraphrase Corpus)**: Sentence pairs annotated for semantic equivalence.
  - **QNLI (Question Natural Language Inference)**: Questions and their corresponding sentences to introduce varied sentence structures.

- **EdinburghNLP/XSum**: Contains abstractive summaries, focusing on concise, varied, and high-quality summary sentences to enhance the diversity of the silver dataset.

### AMR Parsing Model
The AMR3-structbart-Large model was used for generating AMR graphs. Three different seed releases of the model from IBM Research were utilized to create an ensemble distillation, leveraging action sequences to improve the quality of the AMR annotations.

## Download the Dataset
Due to the size of the dataset (1.4GB in total, with individual files up to 300MB), it is hosted on Google Drive. You can download the dataset using the link below:

📦 [Download the Silver AMR Dataset](https://drive.google.com/drive/folders/1qdNhJQQ9VEljP-Asz43iqfDre9rKxbFv?usp=sharing)

Simply follow the link to access and download the full dataset.

## Usage and License
This dataset is open for research and non-commercial use to aid in the advancement of AMR parsing techniques. If you use this dataset in your work, please consider citing the original sources of the GLUE subsets, XSum dataset, and the AMR3-structbart-Large model.

### Citation
When using this dataset, please cite the original papers associated with each component of the dataset:

- **GLUE Benchmark**: [Wang et al. (2019)](https://aclanthology.org/W19-4508/)
- **CoLA**: [Warstadt et al. (2018)](https://aclanthology.org/P18-2124/)
- **MRPC**: [Dolan & Brockett (2005)](https://aclanthology.org/H05-1115/)
- **QNLI**: [Rajpurkar et al. (2016)](https://aclanthology.org/Q16-1002/)
- **XSum Dataset**: [Narayan et al. (2018)](https://aclanthology.org/D18-1206/)
- **AMR3-structbart-Large Model**: [Zhou et al. (2021)](https://aclanthology.org/2021.acl-long.512/)

## Contact
For questions, suggestions, or collaboration opportunities, please reach out through [GitHub Issues](https://github.com/nj19257/AMR-silver-data-for-ensemble-distill/issues).

Happy parsing! 🚀
