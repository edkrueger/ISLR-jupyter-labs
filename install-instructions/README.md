# R for Jupyter Notebooks (with conda)

1) Create the conda environment containering R with `conda create -c r -n <your_env_name> r-base r-essentials`.  
2) Activate the environment with `conda activate <your_env_name>`.  
3) Run `r` in bash to open R in interpretive mode.  

4) Run `IRkernel::installspec(name = '<your_env_name>', displayname = '<your_display_name>')`.  
The `displayname` argument is an optional arguement that specifies the name that is displayed in Jupyter Notebook.  
The `name` argument is the name that appears in the Jupyter Kernelspec; this can be anything, but using the name of the conda environment will make is clearer which conda environment is hooked up with each kernel spec.  

5) Run `quit()` to exit and press the "n" key so you don't save a workspace image.  

6) Open jupyter notebook with `jupyter notebook` in bash.  
7) Either open an existing Jupyter Notebook or create a new one and choose the kernel `<your_display_name>` (or `<your_env_name>` if you declined to specify  