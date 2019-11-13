# Introduction
Code is based on Fairseq 0.6.2, and readme is adapted from the origin readme.
- **parallel multi-scale attention(MUSE)(MUSE)**
  - [Zhao et al. (2019): MUSE: Multi-Scale Attention Model for Sequence to Sequence Learning ](examples/parallel_multi-scale_attention(MUSE)/README.md)

MUSE features:
- Parallel learn multi-scale sequence representations
- First successfully combine convolution and self-attn in one module for sequence tasks by shared projection
- SOTA on three Main translation datasets, WMT14, En-Fr,En-De and IWSLT14 De-En


# Requirements and Installation

* [PyTorch](http://pytorch.org/) version >= 1.0.0
* Python version >= 3.6
* For training new models, you'll also need an NVIDIA GPU and [NCCL](https://github.com/NVIDIA/nccl)

**Installing from source**

To install MUSE from source and develop locally:
```
pip install --editable . --user
```

# Pre-trained models and examples

We provide pre-trained models and detailed example training and
evaluation in examples/parallel_multi-scale_attention(MUSE)/README.md.

# Results
| Task | size  | test (BLEU) |
| ---------- | ---:| ----:|
| IWSLT14 De-En | Base | 36.3 |
| WMT14 En-De |  Large  | 29.9 |
| WMT14 En-Fr |  Large | 43.5 |

# License
MIT-licensed.
The license applies to the pre-trained models as well.
We also provide an additional patent grant.

# Citation

Please cite as:

```bibtex
@inproceedings{
        anonymous2020muse,
        title={{\{}MUSE{\}}: Multi-Scale Attention Model for Sequence to Sequence Learning},
        author={Anonymous},
        booktitle={Submitted to International Conference on Learning Representations},
        year={2020},
        url={https://openreview.net/forum?id=SJe-3REFwr},
        note={under review}
        }
```
