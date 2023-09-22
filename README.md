# PyCon 2023 Workshop: Instruction FineTuning
![icon](./pycon.JPG)

Welcome to the repository. This work is created for participants of a workshop track at [PyCon 2023](https://in.pycon.org/2023/).

There are multiple notebooks available there. Here are short descriptions which may help to quickly follow.

1. `Inference_zero_shot_few_shot_tutorial (Notebook 1)`: This utilizes [Llama-2 7B](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf) and [GPT 3.5 turbo](https://platform.openai.com/docs/models/gpt-3-5) models for predicting sentiment on [Financial statements](https://huggingface.co/datasets/financial_phrasebank). I will be walking over this notebook to develop basic intiution about LLMs and issues with prompt engineering in real case scenarios.

2. `Inference_zero_shot_few_shot_practice (Notebook 2)`: This utilizes Llama-2 7B and GPT 3.5 turbo models for predicting language clarity categories on a [ESG statements](https://huggingface.co/datasets/Abhijeet3922/ESG-Prospectus-Clarity-Category) from Prospectus.  This notebook is meant for participants to practice.

3. `PEFT_Prompt_Tuning_Sentiment (Notebook 3)`: Prompt Tuning is a parameter efficient finetuning technique which utilizes soft tokens (extra parameters) to learn specific task along with utilizing the pretrained knowledge. This demostrates finetuning a LLM with few examples (>1K examples) to get much improved performance. The notebook utilizes [OPT](https://huggingface.co/facebook/opt-1.3b) Language model and sentiment dataset to run over Google [Collab](https://colab.research.google.com/).

4. `PEFT_LORA_Tuning_Sentiment (Notebook 4)`: Low Rank Adaption (LORA) is a popular technique to train low rank adaptor(matrices) on specific task and merge parameters with pretrained language model. This notebook uses same dataset and language model as Notebook 3.

5. `PEFT_Prompt_Tuning_ESG (Notebook 5)`: This practice notebook utilizes OPT model for predicting language clarity categories on a ESG statements from Prospectus.  

6. `PEFT_LORA_Tuning_ESG (Notebook 6)`: This practice notebook utilizes OPT model for predicting language clarity categories on a ESG statements from Prospectus.

7. `Full_FineTuning_LORA_Summarization (Notebook 7)`: This is an instruction finetuning example using [FLAN-T5-base](https://huggingface.co/google/flan-t5-base) model on a sequence to sequence [summarization task](https://huggingface.co/datasets/samsum) which we will walk through in the workshop.


## Installation

Installing these libraries using pip over Google Collab will be sufficient for notebooks to run.

```
accelerate==0.21.0 
bitsandbytes==0.40.2 
transformers==4.31.0
rouge_score==0.1.2
peft==0.4.0
trl==0.4.7
sentencepiece 
xformers 
evaluate
py7zr
```