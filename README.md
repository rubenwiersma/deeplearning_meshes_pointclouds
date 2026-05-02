### Eurographics 2026 Tutorial (2nd edition)
# Deep Learning on Meshes and Point Clouds
Ruben Wiersma

This tutorial accompanies the course/tutorial given at Eurographics 2026 on "Deep Learning on Meshes and Point Clouds". The first edition of this course was given at the SGP 2025 Graduate School.

## Instructions
First, clone the GitHub repository and include the submodules (required for Part 2):
```
git clone --recurse-submodule https://github.com/rubenwiersma/deeplearning_meshes_pointclouds.git
```

**Create a virtual environment**
We'll create an environment to keep our code contained and manageable. You can use any environment manager you like, here the instructions use Python's own `venv` for minimal requirements.

**Note** You'll need at least Python 3.11 for the requirements to install without complaints.

Create the environment in code folder and activate:
```
cd [root_folder]
python -m venv ./dl_venv
source ./dl_venv/bin/activate
```
Whenever you start the tutorial, be sure that the environment is activated!

We then need to install some dependencies. Most important are `torch` and `torch_geometric`. The instructions here assume that you have a CUDA-capable GPU, but you can also run the tutorial on a CPU. In that case, [follow the installation instructions here](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html).

Run the following commands to install `torch`, `torch_geometric` and the rest of the requirements:
```
pip install torch --index-url https://download.pytorch.org/whl/cu126
pip install torch_geometric
pip install pyg_lib torch_cluster -f https://data.pyg.org/whl/torch-2.11.0+cu126.html
pip install -r requirements.txt
```

Then run the notebook:
```
jupyter notebook
```

### Starting the tutorial
The `jupyter notebook` command starts the Jupyter server and opens the Jupyter interface in your browser. If you don't see it, check your terminal for instructions on where to go. It's often located at http://localhost:8889

Then click on `tutorial_part_1.ipynb` in the Jupyter file browser and follow the instructions in the notebook.
Part 2 (`tutorial_part_2.ipynb`) builds on part 1, so be sure to do this _after_ running part 1.
