The **HaVQA_aug** dataset was constructed from the original **HaVQA** dataset through augmentation.  
The table below presents the statistics of this dataset.


| Jeu de données          | Train  | Test  | Images |
|--------------------------|--------|-------|--------|
| HaVQA_aug       | 9 625  | 2 407 | 3 110  |

The authors of the original HaVQA dataset are:
> Shantipriya Parida, Idris Abdulmumin, Shamsuddeen Hassan Muhammad, Aneesh Bose, Guneet Singh Kohli, Ibrahim Said Ahmad, Ketan Kotwal, Sayan Deb Sarkar, Ondřej Bojar, Habeebah Kakudi 
> *HaVQA: Hausa Visual Question Answering Dataset*.  
> [Lien vers l'article](https://aclanthology.org/2023.findings-acl.646/)

👉 The original dataset is available on: [Hugging Face - HaVQA](https://huggingface.co/datasets/HausaNLP/HausaVQA).





| **LLMs** | **Image encoder** | **WuPalmer** | **Accuracy** | **F1-score** |
|-----------|-------------------|--------------|---------------|--------------|
| mT0-base | vit-base-patch16-224-in21k | 15.03% | 15.03% | 0.38% |
| mT0-base | clip-vit-base-patch32 | 14.44% | 14.49% | 0.35% |
| mT0-base | mae-base | 15.37% | 15.38% | 0.37% |
| mT0-base | deit-base-distilled-224 | 15.54% | 15.54% | 0.37% |
| mT0-large | clip-vit-base-patch32 | 15.61% | 15.61% | 0.41% |
| mT0-large | deit-base-distilled-224 | 15.45% | 15.45% | 0.37% |
| afriberta-large | vit-base-patch16-224 | 17.29% | 17.19% | 0.57% |
| afriberta-large | clip-vit-base-patch32 | 17.02% | 17.19% | 0.57% |
| afriberta-large | mae-base | 18.27% | 18.27% | 0.71% |
| afris-bert-large-76L | vit-base-patch16-224 | 17.26% | 16.96% | 0.59% |
| afris-bert-large-76L | clip-vit-base-patch32 | 17.36% | 16.96% | 0.59% |
| afris-bert-large-76L | mae-base | 18.12% | 18.11% | 0.67% |
| gemini | vit-base-patch16-224-in21k | 14.70% | 14.50% | 0.36% |
| gemini | clip-vit-base-patch32 | 14.04% | 14.04% | 0.31% |
| bloomz560 | vit-base-patch16-224-in21k | 17.09% | 17.09% | 0.55% |
| bloomz560 | mae-base | 17.62% | 17.62% | 0.59% |
| bloomz7b1 | vit-base-patch16-224 | 17.36% | 17.36% | 0.59% |
| bloomz7b1 | mae-base | 17.62% | 17.62% | 0.59% |
| bloomz7b1 | deit-base-distilled-224 | 17.25% | 17.25% | 0.56% |
| deepseek-R1-1.5B | vit-base-patch16-224 | 16.11% | 16.11% | 0.47% |
| deepseek-R1-1.5B | clip-vit-base-patch32 | 16.41% | 16.41% | 0.48% |
| deepseek-R1-1.5B | mae-base | 15.84% | 15.84% | 0.45% |
| llama-3.2-1B | vit-base-patch16-224 | **19.04%** | **19.04%** | **1.36%** |
| llama-3.2-1B | clip-vit-base-patch32 | 18.46% | 18.46% | 1.29% |
| llama-3.2-1B | deit-base-patch16-224 | 18.36% | 18.36% | 1.36% |

### Fine-tuning results of LLMs and image encoders on HaVQA dataset
