# OmniEdit
Official Repo for ICLR2025 paper [OmniEdit: Building Image Editing Generalist Models Through Specialist Supervision](https://arxiv.org/abs/2411.07199)

In this paper, we present OMNI-EDIT, which is an omnipotent editor to handle seven different image editing tasks with any aspect ratio seamlessly. Our contribution is in four folds: (1) OMNI-EDIT is trained by utilizing the supervision
from seven different specialist models to ensure task coverage. (2) we utilize importance sampling based on the scores provided by large multimodal models (like GPT-4o) instead of CLIP-score to improve the data quality. 

[📃Paper](https://tiger-ai-lab.github.io/OmniEdit/) | [🌐Website](https://tiger-ai-lab.github.io/OmniEdit/) | [💻Github](https://github.com/TIGER-AI-Lab/OmniEdit) | [📚Dataset](https://huggingface.co/datasets/TIGER-Lab/OmniEdit-Filtered-1.2M)


## Data Pipeline

We synthesize the large scale dataset through specialist distillation. Our synthesis pipeline is depicted in
<p align="center">
<img src="https://huggingface.co/datasets/TIGER-Lab/OmniEdit-Filtered-1.2M/resolve/main/synthesis.png" width="800">
</p>

Our released version contains 1.2M pairs covering seven different skills like addition, swaping, removal, attribute modification, background change, environment change and sytle transfer. The dataset has been filtered with VIEScore.

## Comparison with Others

Our dataset has the most diverse, highest-quality image editing pairs of any resolution.
<p align="center">
<img src="https://huggingface.co/datasets/TIGER-Lab/OmniEdit-Filtered-1.2M/resolve/main/comparison.png" width="800">
</p>


## Citation

If you find our paper useful, please cite us with
```
@article{wei2024omniedit,
  title={OmniEdit: Building Image Editing Generalist Models Through Specialist Supervision},
  author={Wei, Cong and Xiong, Zheyang and Ren, Weiming and Du, Xinrun and Zhang, Ge and Chen, Wenhu},
  journal={arXiv preprint arXiv:2411.07199},
  year={2024}
}
```
