# Simplification via Simultaneous Summarization
This repo is the codes for the NLP course project 

## Installation
Install the required libraries either in the main environment or after making a virtual environment, using

```
pip install -r requirements.txt
```

## Processed Dataset
The datasets used for document-level simplification are listed in `/SimSum/data` , named `D-Wiki` for D-Wikipedia and `wiki_doc` for WikiDoc. We have only used D-Wiki dataset for the study.

## Training
To train the model:
```
python main.py
```

`Bart2.py` and `T5_2.py` means SimSum model with BART and T5 as the backbone `Bart_baseline_finetuned.py` and `T5_baseline_finetuned.py` are single models.


## Automatic Evaluation
To evaluate the model,
```
python evaluate.py
```

which will compute the SARI, D-SARI, FKGL, Rouge-1 and CSS score.
