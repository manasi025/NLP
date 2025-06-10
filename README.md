# NLP
## Use Case 1: Classification Pipeline 
Scenario: Classify customer feedback into “Complaint” vs. “Praise.” 
Tasks: 
1. Prompt & Schema 
o Craft one prompt that ingests raw feedback and returns a JSON {label: 
"Complaint"|"Praise", confidence: float}. 
2. Evaluation 
o On 30 labeled examples, compute precision and recall. Show your 
calculations. 
3. Data Augmentation 
o With an LLM, generate 100 additional “Complaint” examples. Deliver the 
exact prompt and 5 samples. 
4. Error Analysis 
o Given 3 misclassified cases, identify the root cause (e.g., prompt 
ambiguity, class imbalance) and propose a concrete fix (prompt tweak or 
post-processing rule).


## Use Case 2: LLM Fine-Tuning Pipeline 
Scenario: Fine-tune an LLM to summarize technical support tickets into three key 
action items. 
Tasks: 
1. Dataset Preparation 
o From a small corpus of 50 ticket–summary pairs (get a dataset online or 
use LLM to generate), design the JSONL fine-tuning format. Provide 5 
sample records. 
2. Fine-Tuning Plan 
o Choose a base model, outline hyperparameters (learning rate, epochs, 
batch size), and write the CLI (or API) command to launch fine-tuning. 
3. Validation & Metrics 
o On a held-out set of 20 tickets, define and compute ROUGE-1 F1 for 
summaries. Present results. 
4. Iteration & Guardrails 
o Analyze 2 failure cases (e.g., missing action items, verbosity). For each, 
propose a prompt template tweak or post-processing rule to correct it.
