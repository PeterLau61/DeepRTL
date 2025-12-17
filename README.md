# DeepRTL

The official implementation of **DeepRTL: Bridging Verilog Understanding and Generation with a Unified Representation Model (ICLR 2025)**.

## Fine-tuning dataset (released)

We have uploaded the DeepRTL fine-tuning dataset to Hugging Face:  
https://huggingface.co/datasets/liuyi2000/deeprtl_finetuning_dataset

It includes three JSON files:

- **train_data_functional_description.json**: Verilog code paired with **high-level functional descriptions** (*i.e.*, concise summaries of what the module does, with a brief high-level overview of how it works).
- **train_data_specification.json**: Verilog code paired with **detailed specifications**, including both **what it does** and a more **comprehensive explanation of how it works**.
- **train_line_level_comment.json**: **Line-level** data consisting of single-line Verilog statements paired with their corresponding natural-language **inline comments** (filtered to keep comments strictly relevant to their specific lines).

For more details on how these annotations are constructed, please refer to the DeepRTL paper.

## Related dataset: DeepCircuitX (repo-level, complementary)

If you are also interested in **repository-level** RTL data (beyond module-level), please check out **DeepCircuitX**, a concurrent effort from our group. DeepCircuitX is organized across multiple granularities (e.g., repository/file/module/block levels) and is intended for training and evaluation at broader project scope. :contentReference[oaicite:0]{index=0}

- Dataset introduction / access page:  
  https://zeju.gitbook.io/lcm-team/deepcircuitx/introduction-of-our-dataset :contentReference[oaicite:1]{index=1}

In short: **DeepRTL** focuses on **module-level** fine-tuning data, while **DeepCircuitX** provides a more **repo-level** view—so the two datasets are complementary. :contentReference[oaicite:2]{index=2}

## Coming soon

Models, benchmarks, and training/evaluation scripts will be uploaded soon.


