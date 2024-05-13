# awsome-continue-pretraining

## Continual Pre-Training of Large Language Models: How to (re)warm your model?
https://arxiv.org/pdf/2308.04014

Takeaway:
1. The length of the warmup phase does not ap- pear to have a significant effect on the Pile and SlimPajama validation losses.
2.1 Rewarming then decaying the learning rate appears necessary to learn well on the down- stream task. Moreover, while keeping a con- stant learning is initially advantageous on Pile, this advantage vanishes when training long enough on SlimPajama.
2.2 A model that only learns on SlimPajama per- forms worse on SlimPajama than models pre- trained on Pile in spite of being optimised solely for the downstream task, highlighting positive transfer between the two datasets.
3.1 Rewarming the learning rate appears to be a significant cause for the degradation of perfor- mance seen previously when starting to learn on the downstream task, as evidenced by re- warming then decaying the learning rate while training on the same dataset.
3.2 The models donot appear to be able to recover from the performance hit due to rewarming the learning rate when training on the same dataset.
4. Using an earlier checkpoint when pretraining on the Pile does not lead to learning faster on SlimPajama.


## Continual Learning for Large Language Models: A Survey
https://arxiv.org/pdf/2402.01364v2

<img width="1032" alt="image" src="https://github.com/llama-cpt/awsome-continue-pretraining/assets/10681979/cc2fc67e-18aa-419b-be85-e9c3b1ddc1c9">




EMNLP'22 Temporalwiki: A lifelong benchmark for training and evaluating ever-evolving language models.

ICLR'22 Towards continual knowledge learning of language models

ICLR'23 Continual pretraining of language models. 

CoRR'22 Continual pre-training mitigates forgetting in language and vision.

ACL'23Finding Recyclable tuning for continual pre-training.

'24 Pllama: An open-source large language model for plant science

'23 Efficient continual pre-training for building domain specific large language models

Ecomgpt-ct: Continual pre-training of e-commerce large language models with semi-structured data

ACL'21 Learning to solve NLP tasks in an incremental number of languages.

'23 A study of continual learning under language shift.

IJCAI'22 CERT: continual pre-training on sketches for library oriented code generation

ACL'23 Exploring continual learning for code generation models

