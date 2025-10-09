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




| **LLMs** | **Image Encoder** | **WuPalmer** | **Accuracy** | **F1-score** |
|-----------|-------------------|--------------|---------------|--------------|
| mT0-base | vit-base-patch16-224-in21k | 15.85% | 15.86% | 0.38% |
| mT0-base | clip-vit-base-patch32 | 15.37% | 15.37% | 0.37% |
| mT0-base | mae-base | 15.87% | 15.87% | 0.57% |
| mT0-base | deit-base-patch16-224 | 15.87% | 15.87% | 0.37% |
| mT0-large | vit-base-patch16-224-in21k | 16.13% | 16.13% | 0.38% |
| mT0-large | clip-vit-base-patch32 | 16.35% | 16.35% | 0.37% |
| mT0-large | mae-base | 15.96% | 15.96% | 0.41% |
| mT0-large | deit-base-patch16-224 | 16.34% | 16.34% | 0.41% |
| afriberta-large | vit-base-patch16-224 | 19.63% | 19.63% | 0.99% |
| afriberta-large | clip-vit-base-patch32 | 19.56% | 19.56% | 0.90% |
| afriberta-large | mae-base | 19.47% | 19.47% | 0.90% |
| afriberta-large | deit-base-patch16-224 | 19.43% | 19.43% | 0.89% |
| afris-bert-large-76L | vit-base-patch16-224 | 18.80% | 18.80% | 0.81% |
| afris-bert-large-76L | clip-vit-base-patch32 | 18.80% | 18.80% | 0.81% |
| afris-bert-large-76L | mae-base | 18.07% | 18.07% | 0.74% |
| afris-bert-large-76L | deit-base-patch16-224 | 18.07% | 18.07% | 0.74% |
| gemini | vit-base-patch16-224-in21k | 14.54% | 14.52% | 0.36% |
| gemini | clip-vit-base-patch32 | 14.52% | 14.52% | 0.37% |
| bloomz560 | vit-base-patch16-224-in21k | 14.09% | 14.09% | 0.31% |
| bloomz560 | mae-base | 17.49% | 17.49% | 0.75% |
| bloomz7b1 | vit-base-patch16-224-in21k | 18.37% | 18.37% | 0.67% |
| bloomz7b1 | mae-base | 18.37% | 18.37% | 0.67% |
| bloomz7b1 | deit-base-patch16-224 | 18.37% | 18.37% | 0.67% |
| deepseek-R1-1.5B | vit-base-patch16-224 | 18.49% | 18.49% | 1.15% |
| deepseek-R1-1.5B | clip-vit-base-patch32 | 18.49% | 18.49% | 1.15% |
| deepseek-R1-1.5B | mae-base | 15.91% | 15.91% | 0.47% |
| deepseek-R1-1.5B | deit-base-patch16-224 | 15.95% | 15.95% | 0.47% |
| llama-3.2-1B | vit-base-patch16-224-in21k | **17.59%** | **17.59%** | **3.14%** |
| llama-3.2-1B | mae-base | 17.36% | 17.36% | 3.04% |
| llama-3.2-1B | deit-base-patch16-224 | 17.76% | 17.76% | **3.40%** |


### Fine-tuning results of LLMs and image encoders with inline augmentation on HaVQA dataset



| **LLMs** | **Image Encoder** | **WuPalmer** | **Accuracy** | **F1-score** |
|-----------|-------------------|--------------|---------------|--------------|
| mT0-base | vit-base-patch16-224-in21k | 28.07% | 28.04% | 5.97% |
| mT0-base | clip-vit-base-patch32 | 27.25% | 27.54% | 5.41% |
| mT0-base | mae-base | 32.19% | 31.96% | 9.90% |
| mT0-base | deit-base-patch16-224 | 31.94% | 31.94% | 9.86% |
| mT0-large | vit-base-patch16-224-in21k | 34.13% | 34.13% | 14.91% |
| mT0-large | clip-vit-base-patch32 | 34.14% | 34.14% | 14.94% |
| mT0-large | mae-base | 33.02% | 33.25% | 11.45% |
| mT0-large | deit-base-patch16-224 | 31.93% | 31.93% | 11.34% |
| afriberta-large | vit-base-patch16-224 | 32.74% | 32.74% | 13.40% |
| afriberta-large | clip-vit-base-patch32 | 32.74% | 32.74% | 13.40% |
| afriberta-large | mae-base | 33.10% | 33.09% | 13.90% |
| afriberta-large | deit-base-patch16-224 | 31.70% | 31.70% | 13.05% |
| afris-bert-large-76L | vit-base-patch16-224 | 23.07% | 23.07% | 9.35% |
| afris-bert-large-76L | clip-vit-base-patch32 | 24.08% | 24.08% | 9.96% |
| afris-bert-large-76L | mae-base | 26.49% | 26.49% | 11.50% |
| afris-bert-large-76L | deit-base-patch16-224 | 26.94% | 26.94% | 11.91% |
| gemini | vit-base-patch16-224-in21k | **35.85%** | **35.85%** | **15.32%** |
| gemini | clip-vit-base-patch32 | 33.39% | 33.39% | 12.79% |
| gemini | mae-base | 33.39% | 33.39% | 12.79% |
| bloomz560 | vit-base-patch16-224-in21k | 16.13% | 16.12% | 1.41% |
| bloomz560 | clip-vit-base-patch32 | 17.59% | 17.59% | 1.44% |
| bloomz560 | mae-base | 15.51% | 15.12% | 1.16% |
| bloomz560 | deit-base-patch16-224 | 15.83% | 15.84% | 1.17% |
| bloomz7b1 | vit-base-patch16-224-in21k | 17.36% | 17.36% | 2.17% |
| bloomz7b1 | clip-vit-base-patch32 | 18.34% | 18.34% | 2.17% |
| bloomz7b1 | mae-base | 16.17% | 16.17% | 1.74% |
| bloomz7b1 | deit-base-patch16-224 | 16.73% | 16.73% | 1.74% |
| deepseek-R1-1.5B | vit-base-patch16-224-in21k | 18.70% | 18.49% | 1.91% |
| deepseek-R1-1.5B | clip-vit-base-patch32 | 21.10% | 21.09% | 2.07% |
| deepseek-R1-1.5B | mae-base | 15.97% | 15.96% | 2.07% |
| deepseek-R1-1.5B | deit-base-patch16-224 | 15.97% | 15.96% | 2.07% |
| llama-3.2-1B | vit-base-patch16-224-in21k | **17.59%** | **17.59%** | **3.14%** |
| llama-3.2-1B | mae-base | 17.36% | 17.36% | 3.04% |
| llama-3.2-1B | deit-base-patch16-224 | 17.76% | 17.76% | 3.40% |


### Fine-tuning results of offline augmentation on HaVQA dataset






