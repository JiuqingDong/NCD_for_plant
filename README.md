Here's the restructured content using Markdown format:

# NCD_for_plant

## Setup

**Step 1: Create and activate a new conda environment:**
```bash
conda create -n crkd python=3.8
conda activate crkd
```
Install PyTorch and torchvision using pip:
```bash
pip install torch==1.8.1+cu111 torchvision==0.9.1+cu111 -f https://download.pytorch.org/whl/torch_stable.html
```

**Step 2: Install other necessary packages from a requirements file:**
```bash
pip install -r env.txt
pip install gym
pip install umap
```

**Step 3: Check and modify the source code if necessary. Here is the path and required change:**
  - `File Path: anaconda3/envs/uno1/lib/python3.8/site-packages/pl_bolts/datasets/imagenet_dataset.py`
  - Change `from torch._six import PY3` to `from six import PY3`
