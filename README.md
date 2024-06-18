# @Shehzaad: 
### Code to have a look at is the file DPO_NLP_PROJ.ipynb to check if the model can properly get finetuned like we did it or if we made a mistake in our implementation.
# How to replicate our results:
## First Run DPO_NLP_PROJ.ipynb 
this will run DPO on a BART-base model and generate a finetuned version of BART (you can insert a different LLM if your GPU can handle it.)
## Second Run OriginalModelSummaries.ipynb and FineTunedModelSummaries.ipynb
This will generate the summaries that we will compare to the original summaries provided in our dataset by using 1000 validation samples and generating summaries for them with the base and finetuned model.
## Third run DPO_Evaluation.ipynb
This will compute the rouge and bert scores of the generated summaries and compare them to the original (preferred) summaries provided in the dataset for each of the validation samples and allow for a comparison of the DPO´d model and the base model in its summarization capabilities.
