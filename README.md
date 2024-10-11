# Subjective Scoring Framework for VQA Models in Autonomous Driving

This repository provides the code and resources for the paper **["Subjective Scoring Framework for VQA Models in Autonomous Driving"](https://ieeexplore.ieee.org/abstract/document/10536869)** published in **IEEE Access**. The paper introduces a novel framework for subjective evaluation of Visual Question Answering (VQA) models in autonomous driving scenarios. The repository includes the code for the framework and a case study evaluating three VQA models: **ViLBERT**, **ViLT**, and **LXMERT**.

## Abstract

The paper presents a subjective scoring system to assess VQA models specifically for autonomous driving tasks. Traditional accuracy metrics provide a general measure of VQA model performance, but subjective evaluations are needed to fully understand the quality of model-generated answers. The framework evaluates answers based on question subjectivity and uses multiple Natural Language Processing (NLP) models (BERT, NLI-DistilBERT, MPNet, GPT-2) to compute sentence similarity using Cosine Similarity metrics. The case study evaluates three prominent VQA models — ViLBERT, ViLT, and LXMERT — using an automotive dataset to assess their suitability for driving-specific tasks.

## Repository Contents

This repository contains the following files and folders:

```
├── code
│   ├── Subjective_Scoring_Framework.ipynb  # Main implementation of the subjective scoring framework
│   ├── Case_Study.ipynb                    # Case study results for ViLBERT, ViLT, and LXMERT
├── data
│   ├── automotive_dataset/                 # Sample automotive dataset used in the study
│   └── vqa_questions/                      # Set of VQA questions used for evaluation
├── README.md                               # This readme file
└── requirements.txt                        # Python dependencies for the project
```

## Framework Overview

The **Subjective Scoring Framework** provides an in-depth evaluation of VQA models by accounting for question subjectivity. Its key features include:

- **Question Subjectivity Scoring**: The framework adjusts scoring based on the subjectivity level of the questions posed to the models, offering a more refined assessment.
  
- **NLP Models for Answer Comparison**: The framework uses the following models to compare model-generated answers with ground truth:
  - **BERT-base-uncased**
  - **NLI-DistilBERT-base**
  - **All-mpnet-base-v2**
  - **GPT-2**
  
- **Cosine Similarity Metrics**: Measures the similarity between the model-generated answers and the expected answers using sentence embeddings.

## Case Study

The case study evaluates three popular VQA models:
- **ViLBERT**
- **ViLT**
- **LXMERT**

The study uses an automotive dataset to assess how well these models answer questions related to driving scenarios. The subjective scoring framework provides detailed insights into the models' performance, helping identify their strengths and limitations when applied to autonomous driving tasks.

## How to Use

1. **Clone the Repository**:
   ```
   git clone https://github.com/your-repo/subjective-scoring-vqa-autonomous-driving.git
   cd subjective-scoring-vqa-autonomous-driving
   ```

2. **Run the Framework**:
   The **Subjective_Scoring_Framework.ipynb** notebook can be loaded as a stand-alone `.ipynb` file on any coding platform, including **Google Colab**, making it accessible to users without high-capacity GPUs. Upload the notebook to Google Colab or any Jupyter platform and run the cells to evaluate the VQA models using the framework.

3. **Case Study**:
   You can also load the **Case_Study.ipynb** notebook on Google Colab or Jupyter to reproduce the case study results for ViLBERT, ViLT, and LXMERT.

## Results and Insights

The subjective scoring framework offers a detailed evaluation of the VQA models’ performance, highlighting how well they handle driving-specific tasks. The insights gained from the case study help identify the most suitable model for fine-tuning on autonomous driving datasets and highlight areas for improvement in current VQA models.

## Citation

If you use this framework or code in your research, please cite our paper:

```
@article{rekanar2024subjective,
  author={K. Rekanar and A. Ahmed and R. Mohandas and G. Sistu and C. Eising and M. Hayes},
  journal={IEEE Access},
  title={Subjective Scoring Framework for VQA Models in Autonomous Driving},
  year={2024},
  volume={12},
  pages={141306-141323},
  doi={10.1109/ACCESS.2024.3404349}
}
```

## Keywords

- Autonomous vehicles
- Measurement
- Visualization
- Analytical models
- Intelligent vehicles
- Data models
- Task analysis
- Semantics
- Question answering (information retrieval)
- Semantic analysis
- Scoring framework
- Subjective assessment
- VQA models

## License

This project is licensed under a **Creative Commons License**.

## Acknowledgments

This publication has emanated from research supported in part by a grant from **Science Foundation Ireland** under Grant number **18/CRT/6049**. For the purpose of Open Access, the author has applied a **CC BY public copyright license** to any Author Accepted Manuscript version arising from this submission.

We would also like to thank the developers of the NLP models used in this framework, and the research community for their contributions to VQA models and autonomous driving technologies. Special thanks to the creators of the automotive dataset used in the case study.

---

For any issues or questions, please open an issue on this repository.
