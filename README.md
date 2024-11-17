# ColPali Cookbooks 👨🏻‍🍳

[![GitHub](https://img.shields.io/badge/ColPali_Cookbooks-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/tonywu71/colpali-cookbooks)
[![arXiv](https://img.shields.io/badge/arXiv-2407.01449-b31b1b.svg?style=for-the-badge)](https://arxiv.org/abs/2407.01449)
[![Hugging Face](https://img.shields.io/badge/Vidore-FFD21E?style=for-the-badge&logo=huggingface&logoColor=000)](https://huggingface.co/vidore)
[![X](https://img.shields.io/badge/Thread-%23000000?style=for-the-badge&logo=X&logoColor=white)](https://x.com/tonywu_71/status/1809183824464560138)

[[ColPali Engine]](https://github.com/illuin-tech/colpali)
[[ViDoRe Benchmark]](https://github.com/illuin-tech/vidore-benchmark)

## Introduction

With our new model *ColPali*, we propose to leverage VLMs to construct efficient multi-vector embeddings in the visual space for document retrieval. By feeding the ViT output patches from PaliGemma-3B to a linear projection, we create a multi-vector representation of documents. We train the model to maximize the similarity between these document embeddings and the query embeddings, following the ColBERT method.

Using ColPali removes the need for potentially complex and brittle layout recognition and OCR pipelines with a single model that can take into account both the textual and visual content (layout, charts, ...) of a document.

This repository contains notebooks for learning about the ColVision family of models, fine-tuning them for your specific use case, creating similarity maps to interpret their predictions, and more! 😍

| Task             | Notebook                                                     | Description                                                  |
| ---------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Interpretability | [ColPali: Generate your own similarity maps](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/gen_colpali_similarity_maps.ipynb) | Generate your own similarity maps to interpret ColPali's predictions. |
| Interpretability | [ColQwen2: Generate your own similarity maps](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/gen_colqwen2_similarity_maps.ipynb) | Generate your own similarity maps to interpret ColQwen2's predictions. |
| Fine-tuning      | [Fine-tune ColPali](https://github.com/tonywu71/colpali-cookbooks/blob/main/examples/finetune_colpali.ipynb) | Fine-tune ColPali using LoRA and optional 4bit/8bit quantization. |
| RAG              | [ColQwen2: One model for your whole RAG pipeline with adapter hot-swapping 🔥](https://colab.research.google.com/github/tonywu71/colpali-cookbooks/blob/main/examples/run_e2e_rag_colqwen2_with_adapter_hot_swapping.ipynb) | Save VRAM by using a VLM for your entire RAG pipeline.       |

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
