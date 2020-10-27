# TABLE TO TEXT With Logic

Table to text is a model based on GPT2 to convert open domain tables to text.
It is based on the paper
[Logical Natural Language Generation from Open-Domain Tables](https://arxiv.org/abs/2004.10404), which aims to study the problem of natural language generation with logical inference in the intermediate steps. Going beyond simply surface-level copying.

## Requirements
- pytorch 1.4.0
- huggingface transformers 2.5.1
- tensorboardX
- tqdm

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

```bash
pip install -r requirements.txt
sh prerun.sh
```

## Usage

```
CUDA_VISIBLE_DEVICES=0 python GPT2.py --do_test_once\
 --load_from models/GPT_ep8.pt \
--title Stock \
--csv_path mycsv.csv
```
