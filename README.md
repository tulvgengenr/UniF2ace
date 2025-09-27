# UniF²ace: A Unified Fine-grained Face Understanding and Generation Model

[![ArXiv](https://img.shields.io/badge/Arxiv-<2503.08120>-<COLOR>.svg)](https://arxiv.org/abs/2503.08120) [![Project](https://img.shields.io/badge/ProjectPage-UniF²ace-<COLOR>.svg)](https://tulvgengenr.github.io/UniF2ace-Project-Page/) [![Dataset](https://img.shields.io/badge/Dataset-HuggingFace-<COLOR>.svg)](https://huggingface.co/datasets/tulvgengenr/UniF2ace-130K)

UniF²ace is the first unified multimodal model specifically designed for face understanding and generation, encompassing tasks such as visual question answering, face image captioning and text-to-face image generation. 

![overview](assets/overview.png)

This repository contains code for the paper [UniF²ace: A Unified Fine-grained Face Understanding and Generation Model](https://arxiv.org/abs/2503.08120).

## 🎉 Key Contributions
+ A unified face understanding and generation framework: We introduce UniF²ace, the first unified multimodal model for fine-grained face understanding and generation, establishing a solid baseline. 

+ A novel Dual Discrete Diffusion (D3Diff) loss function and a hybrid MoE architecture: We introduce D3Diff, a novel loss function within that theoretically unifies score-based diffusion and masked generative models, leading to a better approximation of the negative log-likelihood for high-fidelity generation and fine-grained attribute control. Additionally, we explore a hybrid Mixture-of-Experts (MoE) architecture at the token and sequence levels, adaptively incorporating the semantic and identity facial embeddings to complement the attribute forgotten phenomenon in representation evolvement.

+ We construct UniF²aceD-1M, a dataset containing 1M VQAs with an automated pipeline. Extensive experiments demonstrate that UniF²ace significantly outperforms or is on par with existing state-of-the-art models with a similar scale on various benchmarks, all while providing a more unified and efficient solution.

## 🔥 News

2025.07.15 We have released the fine-grained face dataset [UniF²aceD-1M](https://huggingface.co/datasets/tulvgengenr/UniF2ace-130K) with captions and VQAs !

![dataset](assets/dataset.png)

## Citation
```latex
@article{li2025unif2ace,
  title={Unif2ace: Fine-grained face understanding and generation with unified multimodal models},
  author={Li, Junzhe and Qiu, Xuerui and Xu, Linrui and Guo, Liya and Qu, Delin and Long, Tingting and Fan, Chun and Li, Ming},
  journal={arXiv preprint arXiv:2503.08120},
  year={2025}
}
```

## License

All code within this repository is under [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
