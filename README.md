# ColPali Cookbooks 👨🏻‍🍳

[![GitHub](https://img.shields.io/badge/ColPali_Cookbooks-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/tonywu71/colpali-cookbooks)
[![arXiv](https://img.shields.io/badge/arXiv-2407.01449-b31b1b.svg?style=for-the-badge)](https://arxiv.org/abs/2407.01449)
[![Hugging Face](https://img.shields.io/badge/Vidore-FFD21E?style=for-the-badge&logo=huggingface&logoColor=000)](https://huggingface.co/vidore)
[![X](https://img.shields.io/badge/Thread-%23000000?style=for-the-badge&logo=X&logoColor=white)](https://x.com/tonywu_71/status/1809183824464560138)

[[ColPali Engine]](https://github.com/illuin-tech/colpali)
[[ViDoRe Benchmark]](https://github.com/illuin-tech/vidore-benchmark)

## Introduction

[ColPali](https://huggingface.co/papers/2407.01449) is a model designed to retrieve documents by analyzing their visual features. Unlike traditional systems that rely heavily on text extraction and OCR, ColPali treats each page as an image. It uses [Paligemma-3B](./paligemma) to capture not only text, but also the layout, tables, charts, and other visual elements to create detailed multi-vector embeddings that can be used for retrieval by computing pairwise late interaction similarity scores. This offers a more comprehensive understanding of documents and enables more efficient and accurate retrieval.

This repository contains notebooks for learning about the ColVision family of models, fine-tuning them for your specific use case, creating similarity maps to interpret their predictions, and more! 😍

## Table of Contents

You can find the cookbooks in the [`examples`](https://github.com/tonywu71/colpali-cookbooks/tree/main/examples) directory. In the table below, they are listed from most recent to oldest.

| Task                        | Notebook                                                                                                                                                                                              | Description                                                                                            |
|-----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| Inference, interpretability | [Use the 🤗 transformers-native ColQwen2](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/use_transformers_native_colqwen2.ipynb)                                                      | Use the 🤗 transformers-native implementation of ColQwen2 for inference, scoring, and interpretability. |
| Inference, interpretability | [Use the 🤗 transformers-native ColPali](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/use_transformers_native_colpali.ipynb)                                                      | Use the 🤗 transformers-native implementation of ColPali for inference, scoring, and interpretability. |
| RAG                         | [ColQwen2: One model for your whole RAG pipeline with adapter hot-swapping 🔥](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/run_e2e_rag_colqwen2_with_adapter_hot_swapping.ipynb) | Save VRAM by using a unique VLM for your entire RAG pipeline. Works even on Colab's free T4 GPU!       |
| Interpretability            | [ColQwen2: Generate your own similarity maps 👀](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/gen_colqwen2_similarity_maps.ipynb)                                                 | Generate your own similarity maps to interpret ColQwen2's predictions.                                 |
| Interpretability            | [ColPali: Generate your own similarity maps 👀](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/gen_colpali_similarity_maps.ipynb)                                                   | Generate your own similarity maps to interpret ColPali's predictions.                                  |
| Fine-tuning                 | [Fine-tune ColPali 🛠️](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/finetune_colpali.ipynb)                                                                                      | Fine-tune ColPali using LoRA and optional 4bit/8bit quantization.                                      |

## Instructions

### Open with Colab

The easiest way to use the notebooks is to open them from the `examples` directory and click on the Colab button below:

![Colab](https://img.shields.io/badge/Open_in_Colab-F9AB00?logo=googlecolab&logoColor=fff&style=for-the-badge)

This will open the notebook in Google Colab, where you can run the code and experiment with the models.

### Run locally

If you prefer to run the notebooks locally, you can clone the repository and open the notebooks in Jupyter Notebook or in your IDE.

## Citation

**ColPali: Efficient Document Retrieval with Vision Language Models**  

Authors: **Manuel Faysse**\*, **Hugues Sibille**\*, **Tony Wu**\*, Bilel Omrani, Gautier Viaud, Céline Hudelot, Pierre Colombo (\* denotes equal contribution)

```latex
@misc{faysse2024colpaliefficientdocumentretrieval,
      title={ColPali: Efficient Document Retrieval with Vision Language Models}, 
      author={Manuel Faysse and Hugues Sibille and Tony Wu and Bilel Omrani and Gautier Viaud and Céline Hudelot and Pierre Colombo},
      year={2024},
      eprint={2407.01449},
      archivePrefix={arXiv},
      primaryClass={cs.IR},
      url={https://arxiv.org/abs/2407.01449}, 
}
```
