### Train and test set:
Train set: 12178 cases
Test set: 3044 cases

### Fine-tuning data:
Training set: 10961 cases (90% of Train set) <br /> 
Validation set: 1217 cases (10% of Train set)
| Case Name | Input | Output | Label | Count | Decision Count | text |
|----------|----------|----------|----------|----------|----------|----------|
| Petitioner vs. Respondent | Case Text | Case Decision[ds]Explanation | Case Decision | Tokens in case text | Tokens in Explanation text | Prompt for fine-tuning |

Prompt for prediction:
```
Here is an instruction that describes a task, paired with an input (Case text) that provides further context. The case decision is given.

### Instruction:
{instruction}

### Input:
{case_text}

### Response:
{case_decision}
```

 
Prompt for prediction and explanation:
```
Here is an instruction that describes a task, paired with an input (Case text) that provides further context. The case decision and explanation for the decision are given.

### Instruction:
{instruction}

### Input:
{case_text}

### Response:
{case_decision}

### Explanation:
{explanation}
```

* val_1217
  * [LLAMA-2-7B_prediction_with_1000_words_input.csv](https://drive.google.com/file/d/1qrwrTMV5HVKvYmkyG5AMCY5owjbFZxsw/view?usp=sharing)
  * [LLAMA-2-7B_prediction_explanation_with_1000_words_input_1000_words_explanation.csv](https://drive.google.com/file/d/12w-jyO9cASUk8R2C1B3H0799SctJ4p4z/view?usp=sharing)
