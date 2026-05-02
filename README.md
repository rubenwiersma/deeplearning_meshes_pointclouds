### Eurographics 2026 Tutorial (2nd edition)
# Deep Learning on Meshes and Point Clouds
Ruben Wiersma

This tutorial accompanies the course/tutorial given at Eurographics 2026 on "Deep Learning on Meshes and Point Clouds". The first edition of this course was given at the SGP 2025 Graduate School.

## Instructions
[Skip to instructions for Visual Studio Code](#alternative-in-visual-studio-code)

For this tutorial, you'll need to install Jupyter in your Python environment. We will install the rest of the required packages from the notebook, so you can also run the code on online services like Google Colab.


**Create a virtual environment**
We'll create an environment to keep our code contained and manageable. You can use any environment manager you like, here the instructions use Python's own `venv` for minimal requirements.

Create the environment in code folder and activate:
```
cd [root_folder]
python -m venv ./dl_tutorial
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

Then click on `sgp_dl_tutorial.ipynb` in the Jupyter file browser and follow the instructions in the notebook.

### Alternative in Visual Studio Code
You can also run the notebook within Visual Studio Code. First, create the conda environment with the right Python version and Jupyter:
```bash
conda create -n sgp_dl python=3.12 jupyter
```

Then, open `sgp_dl_tutorial.ipynb` in Visual Studio Code, select the `sgp_dl` environment in the top-right corner ("Select Kernel" $\rightarrow$ "Python Environments") and go through the notebook step-by-step. If you didn't use conda, but installed Jupyter in your default Python installation, you can select that environment (if you don't know where it's installed, run `which python` in your terminal).
