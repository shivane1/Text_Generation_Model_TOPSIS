# TOPSIS Method for Selecting the Best Pretrained Model for Text Generation

## Overview
This project implements the **TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution)** method to evaluate and rank pretrained models for text generation based on multiple performance criteria.

## 1. Models and Evaluation Criteria
The following pretrained models are evaluated:
- **GPT-3**
- **GPT-2**
- **BERT**
- **T5**
- **BART**

The criteria for evaluation include:
- **Perplexity** (Lower is better)
- **BLEU Score** (Higher is better)
- **Inference Time** (Lower is better)
- **Model Size** (Lower is better)

### Decision Matrix
| Model   | Perplexity | BLEU Score | Inference Time (s) | Model Size (MB) |
|---------|------------|------------|--------------------|-----------------|
| GPT-3   | 20         | 40         | 2.0                | 3500            |
| GPT-2   | 30         | 35         | 1.5                | 1500            |
| BERT    | 25         | 30         | 0.8                | 1200            |
| T5      | 22         | 33         | 1.2                | 1100            |
| BART    | 28         | 37         | 1.0                | 1600            |

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
![Ranking Screenshot](https://github.com/user-attachments/assets/ac4bed92-b9d3-4e6e-af95-adb984274574)

### TOPSIS Output:
![TOPSIS Output](https://github.com/user-attachments/assets/7d970be5-ed8c-4088-ad42-71698b60dd97)

## 5. Usage
1. Clone this repository.
2. Run `Modified_TOPSIS_Text_Generation_Model_Selection.ipynb` in Jupyter Notebook.
3. Modify the dataset to evaluate different models.

## 6. Conclusion
Using the **TOPSIS method**, we effectively ranked pretrained models for text generation based on multiple criteria, providing a systematic approach for model selection.
"""

# Save README file
with open("SHIVANE_KAPOOR_102203191_README.md", "w", encoding="utf-8") as f:
    f.write(readme_content)

print("SHIVANE_KAPOOR_102203191_README.md file has been generated successfully!")
