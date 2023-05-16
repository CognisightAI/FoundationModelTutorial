# Foundation Model Tutorial
A outline and set of links for beginner to learn about current Foundation Models(FM)

## Transformers and Attention

Attention machanism serve as the foundamental building block of modern FM. Though in many cases the variation instead of the original degisn is used, but the key idea and main flow remains the same.

### Material

The **[annotated-transformer](https://github.com/harvardnlp/annotated-transformer/tree/master)** by Harvard.

### Task

Go through the [codes](https://github.com/harvardnlp/annotated-transformer/blob/master/AnnotatedTransformer.ipynb) and understand how Attention and transformers work. Also getting a basic grasp on what is encoder and what is decoder

## LLM

Knowing the famous branchs of Large Language Models(LLM)



### [GPT3](https://proceedings.neurips.cc/paper/2020/file/1457c0d6bfcb4967418bfb8ac142f64a-Paper.pdf) and Prompting(aka. `In-Context Learning`)

### Material

The [paper](https://proceedings.neurips.cc/paper/2020/file/1457c0d6bfcb4967418bfb8ac142f64a-Paper.pdf) for GPT-3.

### Task

Go over the basic trainings so you know what is the most class LLM, GPT-3 is trained with. You should also know GPT-3 is what invented Prompt, so I hope you can gain a basic understanding of what prompt is how hard it was for using prompts to use LLM before `Instruction Tuning`.

*Note:* Before you begin with LLaMA, I would strongly recomment for you to jump to the section below for **Scaling Law** and understand Scaling Law before you continue.

### [LLaMA](https://ar5iv.labs.arxiv.org/html/2302.13971v1) by Meta

LLaMA used many classic designs. and is released to be one of the currently major branches in reproducing ChatGPT.

#### Matrial

See the [paper](https://ar5iv.labs.arxiv.org/html/2302.13971v1) for LLaMA

#### Task

Understanding each module's technique selected by LLaMA, and Taking a note about the data it used.

### (Optional) Survey

#### Material

Surveys about FM/Large Model, e.g. https://arxiv.org/pdf/2302.09419.pdf

#### Task

Compare your understanding with others. understand ways of categorizing FM and list down the differences between different FM.

## Scaling Law

*Pre-requiries* By this time, you should know what is `Pre-Training` is for and can tell the difference between Fine-Tuning and Pre-Training

Scaling Law is specially important when training larger models. As in most cases you won't have enough resources and time to optimize the hyper-parameters, you will have to estimate how much data you need for your model.

There are 2 versions of scaling law, we will be introducing the second version.

### Material

The chinchilla [paper](https://ar5iv.labs.arxiv.org/html/2203.15556).

### Task

Go over the paper and understand the conclusion.

## Instruction Model

### Classic Instruction

[InstructGPT/TextDavinci_002~003](https://proceedings.neurips.cc/paper_files/paper/2022/file/b1efde53be364a73914f58805a001731-Paper-Conference.pdf)

You should understand the three step approach( `pretraining` --> `sft` --> `rlhf` ) for Instruction Tunning by OpenAI(You can skip PPO algorithm, but you should know what is RL for).

Also Jump into the appendix session and look at the labeling instructions given to the labelers during RM's data labeling

### Chat Instruction

Understand that classic approachs beginning with ChatGPT

[ChatGPT](TODO) (ChatGPT's paper is not out yet, but OpenAI claims that they used similar strategy as InstructGPT)

[Alpaca](https://github.com/tatsu-lab/stanford_alpaca/) by stanford

### Other Repositories

[MiniGPT-4](https://github.com/Vision-CAIR/MiniGPT-4#getting-started)

[DeepSpeed-Chat](https://github.com/microsoft/DeepSpeedExamples/tree/master/applications/DeepSpeed-Chat)

