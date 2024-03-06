“Gemma, a family of lightweight, state-of-the art open models built from the research and technology used to create Gemini models.”

**What’s special with Gemma ?**
Lightweight 
 faster inference speeds and lower computational demands
Open source 
Open-Source Availability, customisable , fine tune 
Responsible  AI 
safely aligned open models, safely curated training data to filter any harmful content 
High evaluation bar on resp AI areas
Red teaming 
https://blog.google/technology/developers/gemma-open-models/ 

**Gemma Performance **
Surpasses significantly larger models on key benchmarks while adhering to our rigorous standards for safe and responsible outputs. Refer : https://ai.google.dev/gemma 
Source : https://storage.googleapis.com/deepmind-media/gemma/gemma-report.pdf


**Pretrained weights checkpoints **
gemma_2b_en
gemma_7b_en

**Fine-tuned weights checkpoints**
gemma_instruct _2b_en
gemma_instruct _7b_en

**How has Gemma emphasised Responsible AI ?**
Training 	
  Filtering & careful data
Evaluation 
  Against multiple Resp ai dataset 
Responsbile AI 
  Toolkit Guide 
  Learning Interpretability tool
  Safety Classifiers 
    Perspective API 
    Text moderation service 

**Gemma Architecture**
The Gemma model architecture is based on the transformer decoder
Follows same architecture of Gemini  
“CORE COMPONENTS”
Multi-Query Attention 
RoPE Embeddings
GeGLU Activations 
Normalizer Location

**Gemma Training**

PRETRAINING
GEMMA 2B - 2T Tokens
GEMMA 7B - 6T Tokens
Source : Primarily-English data sourced from Web Docs, mathematics, and code.
Responsible AI 
careful filtering process to remove Unwanted or Unsafe Content, including personal information and sensitive data.


INSTRUCTION FINETUNING

1.Supervised Finetuning(SFT)
text-only, English-only synthetic, and human-generated prompt-response pairs , LM-based side-by-side evaluations on superior models ,LM-based judges

2. RLHF
used variant of reinforce with human feedback 

Model Training and Optimisation

Hardware : 

TPUv5e

TPUv5e are deployed in pods of 256 chips, 
configured into a 2D torus of 16 x 16 chips.
Optimiser
The optimizer state is further sharded using techniques
 similar to ZeRO-3. Beyond a pod, we perform 
data replica reduce over the data-center network
, using Pathways approach”


Consent form https://www.kaggle.com/models/google/gemma/license/consent
Gemma base generation https://colab.research.google.com/github/google/generative-ai-docs/blob/main/site/en/gemma/docs/get_started.ipynb#scrollTo=aL6PJMaE39rc 
No-code models try out 
https://www.kaggle.com/models/keras/gemma/frameworks/keras/variations/gemma_instruct_7b_en 
Finetune Gemma  using LORA. 
https://github.com/GoogleCloudPlatform/vertex-ai-samples/blob/main/notebooks/community/model_garden/model_garden_gemma_kerasnlp_to_vertexai.ipynb 
LIT  (Learning Interpretability Tool)
https://codelabs.developers.google.com/codelabs/responsible-ai/lit-gemma#10 









