# CS701 Tutorial · LoRA for a Pretrained ViT

CS701 (SMU), Week 10 tutorial, 23 Oct 2026 · TA Zichen

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/doem97/cs701-w10-lora-tutorial/blob/main/W10_T1_lora_for_vit.ipynb)

In this notebook, you adapt one pretrained ViT-B/16 to a small dataset in three ways:
linear probe, full fine-tuning and LoRA. You write LoRA yourself (about 15 lines).

## How to run

1. Click **Open in Colab** above.
2. **File → Save a copy in Drive.**
3. **Runtime → Change runtime type → T4 GPU.**
4. Run the cells from the top, one by one.

Each training cell takes about one minute on the free T4.
Your numbers can differ a little from the slides.

## Files

| file | what |
|---|---|
| `W10_T1_lora_for_vit.ipynb` | the notebook (no outputs): open this one |
| `W10_T1_lora_for_vit_with_outputs.ipynb` | the same notebook, run by the TA, with all outputs |

## Data

The notebook downloads a small EuroSAT subset (10 classes, 200 training and 1,000 test images, 4 MB) from
https://huggingface.co/datasets/doem1997/cs701-w10-lora-data.
EuroSAT: Helber et al., 2019, MIT licence.

## Your assignment

The `LoRA` class in this notebook is the same as the class in `sarbench/adapters.py` of the assignment code
(https://github.com/doem97/cs701-sar-benchmark).
