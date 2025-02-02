# TOPSIS Method for Selecting the Best Pretrained Model for Text Generation

## Overview
This project implements the **TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution)** method to evaluate and rank pretrained models for text generation based on multiple performance criteria.

## 1. Models and Evaluation Criteria
The following pretrained models are evaluated:
- **LLaMA**
- **Falcon**
- **Mistral**
- **Gemini**
- **Claude**

The criteria for evaluation include:
- **ROUGE Score** (Higher is better)
- **METEOR Score** (Higher is better)
- **Inference Time (seconds)** (Lower is better)
- **Memory Usage (GB)** (Lower is better)

### Decision Matrix
| Model   | ROUGE Score | METEOR Score | Inference Time (s) | Memory Usage (GB) |
|---------|------------|-------------|--------------------|-----------------|
| LLaMA   | 55         | 0.45        | 1.8                | 10.0            |
| Falcon  | 50         | 0.42        | 1.4                | 8.0             |
| Mistral | 48         | 0.39        | 0.9                | 7.0             |
| Gemini  | 52         | 0.44        | 1.3                | 9.0             |
| Claude  | 49         | 0.41        | 1.1                | 8.5             |

## 2. Implementation Steps
The **TOPSIS method** is applied using the following steps:
1. **Normalization** of the decision matrix.
2. **Weighted normalization** of the decision matrix.
3. **Calculation of ideal best and worst solutions**.
4. **Distance computation** from the ideal solutions.
5. **Calculation of TOPSIS scores** for each model.
6. **Ranking of models** based on the scores.

## 3. Code Execution
The implementation is provided in the Jupyter Notebook: `Modified_TOPSIS_Text_Generation_Model_Selection.ipynb`.

## 4. Results
### Final Rankings:
| Rank | Model  | TOPSIS Score |
|------|--------|--------------|
| 1    | Gemini | 0.5577       |
| 2    | Mistral| 0.5145       |
| 3    | LLaMA  | 0.4855       |
| 4    | Falcon | 0.4808       |
| 5    | Claude | 0.4583       |

### TOPSIS Output:
A bar chart is generated to visualize the rankings.

## 5. Usage
1. Clone this repository.
2. Run `Modified_TOPSIS_Text_Generation_Model_Selection.ipynb` in Jupyter Notebook.
3. Modify the dataset to evaluate different models.

## 6. Conclusion
Using the **TOPSIS method**, we effectively ranked pretrained models for text generation based on multiple criteria, providing a systematic approach for model selection.



## Results
### Final Rankings:
![image](https://github.com/user-attachments/assets/896d251c-47eb-4ceb-867c-5a81c8ccec67)


### TOPSIS Output:
![image](https://github.com/user-attachments/assets/1698dbaf-8c50-4273-a20b-9c55ef9aa08a)
