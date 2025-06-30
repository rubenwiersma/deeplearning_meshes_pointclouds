### SGP 2025 Graduate School
# Deep learning on meshes and point clouds
Ruben Wiersma

## Instructions
[Skip to instructions for Visual Studio Code](#alternative-in-visual-studio-code)

For this tutorial, you'll need to install Jupyter in your Python environment. We will install the rest of the required packages from the notebook, so you can also run the code on online services like Google Colab.

**Option 1 (only pip)**

Install jupyter:
```bash
pip install jupyter
```
To run the notebook:
```
cd [root_folder]
jupyter notebook
```

**Option 2 (separate environment with conda)**

If you have conda installed ([instructions on how to install Miniconda](https://www.anaconda.com/docs/getting-started/miniconda/install)), you can run the following command in your terminal to create the right environment and install jupyter:
```bash
conda create -n sgp_dl python=3.12 jupyter
```
To run the notebook:
```bash
cd [root_folder]
conda activate sgp_dl
jupyter notebook
```

### Starting the tutorial
The `jupyter notebook` command starts the Jupyter server and opens the Jupyter interface in your browser. If you don't see it, check your terminal for instructions on where to go. It's often located at http://localhost:8889

Then click on `sgp_dl_tutorial.ipynb` in the Jupyter file browser and follow the instructions in the notebook.

### Alternative in Visual Studio Code
You can also run the notebook within Visual Studio Code. Simply open `sgp_dl_tutorial.ipynb` in Visual Studio Code, select the `sgp_dl` environment in the top-right corner ("Select Kernel" $\rightarrow$ "Python Environments") and go through the notebook step-by-step.