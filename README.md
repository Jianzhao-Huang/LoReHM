# LoReHM
Official PyTorch implementation for the paper - **Towards Low-Resource Harmful Meme Detection with LMM Agents**.

(**EMNLP 2024**: *The 2024 Conference on Empirical Methods in Natural Language Processing, Nov 2024, Miami, Florida*.) [[`paper`](https://aclanthology.org/2024.emnlp-main.136.pdf)]

## Install

1. Clone the repo
```
git clone https://github.com/Jianzhao-Huang/LoReHM.git
cd LoReHM
```

2. Install Package
```
conda create -n lorehm python=3.10 -y
conda activate lorehm
pip install -r requirements.txt
```

## Dataset

Please obtain FHM, HarM, and MAMI, and place them in the following directories: 

- LoReHM/datasets/FHM
- LoReHM/datasets/harmC
- LoReHM/datasets/MAMI

## Inference
Edit the command line args to change inference settings.

```
python main.py \
--dataset_name FHM \
--model 'llava-v1.6-34b' \
--rsa \
--mia
```

## Citation

```
@inproceedings{huang2024towards,
  title={Towards Low-Resource Harmful Meme Detection with LMM Agents},
  author={Huang, Jianzhao and Lin, Hongzhan and Ziyan, Liu and Luo, Ziyang and Chen, Guang and Ma, Jing},
  booktitle={Proceedings of the 2024 Conference on Empirical Methods in Natural Language Processing},
  pages={2269--2293},
  year={2024}
}
```
