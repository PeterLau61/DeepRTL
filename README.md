# DeepRTL
The official implementation of DeepRTL: Bridging Verilog Understanding and Generation with a Unified Representation Model (ICLR 2025).

## Fine-tuning dataset
We have uploaded the DeepRTL fine-tuning dataset to Hugging Face:
https://huggingface.co/datasets/liuyi2000/deeprtl_finetuning_dataset

It includes three JSON files:

- train_data_functional_description.json: Verilog code paired with high-level functional descriptions (*i.e.*, concise summaries of what the module does, with a brief high-level overview of how it works).
- train_data_specification.json: Verilog code paired with detailed specifications, including both what it does and a more comprehensive explanation of how it works.
- train_line_level_comment.json: Line-level data consisting of single-line Verilog statements paired with their corresponding natural-language inline comments (filtered to keep comments strictly relevant to their specific lines).

For more details on how these annotations are constructed, please refer to the [DeepRTL paper](https://arxiv.org/pdf/2502.15832).

## Understanding benchmark
We have uploaded the DeepRTL **understanding benchmark** to this GitHub repository.

## Related dataset: DeepCircuitX (repo-level, complementary)
If you are also interested in repository-level RTL data (beyond module-level), please check DeepCircuitX, a concurrent effort from our group. DeepCircuitX is organized across multiple granularities (*e.g.*, repository/file/module/block levels) and is intended for training and evaluation at broader project scope.

Dataset introduction / access page:
https://zeju.gitbook.io/lcm-team/deepcircuitx/introduction-of-our-dataset

In short: DeepRTL focuses on module-level fine-tuning data, while DeepCircuitX provides a repo-level view, so the two datasets are complementary.

## Citation

If you find our work useful, please consider citing:

```bibtex
@inproceedings{liudeeprtl,
  title={DeepRTL: Bridging Verilog Understanding and Generation with a Unified Representation Model},
  author={Liu, Yi and Xu, Changran and Zhou, Yunhao and Li, Zeju and Xu, Qiang},
  booktitle={The Thirteenth International Conference on Learning Representations},
  year={2025}
}

@inproceedings{liu2025deeprtl2,
  title={DeepRTL2: A Versatile Model for RTL-Related Tasks},
  author={Liu, Yi and Zhang, Hongji and Zhou, Yunhao and Shi, Zhengyuan and Xu, Changran and Xu, Qiang},
  booktitle={Findings of the Association for Computational Linguistics: ACL 2025},
  year={2025}
}

@inproceedings{li2025deepcircuitx,
  title={Deepcircuitx: A comprehensive repository-level dataset for rtl code understanding, generation, and ppa analysis},
  author={Li, Zeju and Xu, Changran and Shi, Zhengyuan and Peng, Zedong and Liu, Yi and Zhou, Yunhao and Zhou, Lingfeng and Ma, Chengyu and Zhong, Jianyuan and Wang, Xi and others},
  booktitle={2025 IEEE LLM Aided Design Workshop (LAD)},
  year={2025},
  organization={IEEE}
}
