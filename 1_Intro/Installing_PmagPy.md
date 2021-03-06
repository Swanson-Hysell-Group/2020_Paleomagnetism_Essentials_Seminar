# Installing PmagPy

## Install miniconda

Install a **Python 3.7** version of miniconda:
https://docs.conda.io/en/latest/miniconda.html

## Install jupyterlab

Use the terminal or an Anaconda Prompt to install Jupyter:

```
conda install jupyterlab
```

## Create a PmagPy environment from the environment.yml file

Use the terminal or an Anaconda Prompt for the following steps:

- Create the environment from the ``environment.yml`` file:

```
conda env create -f environment.yml
```

   The first line of the ``yml`` file sets the new environment's
   name. For details see :ref:`Creating an environment file manually
   <create-env-file-manually>`.


- Activate the new environment: ``conda activate pmagpy_miniconda``

- Verify that the new environment was installed correctly:

```
conda env list
```

  You can also use ``conda info --envs``.

 - Verify that PmagPy is functioning:

```
ipython     
In [1]: import pmagpy.ipmag as ipmag
In [2]: ipmag.igrf([2020,0,37.87, -122.27])
 ```

 You should see
 ```
Out[2]: array([1.37988492e+01, 6.13403282e+01, 4.86139947e+04])
 ```

 You can then quit out of the ipython prompt:
 ```
In [3]: ipmag.igrf([2020,0,37.87, -122.27])
 ```

 ## Add the PmagPy environment to your Jupyter kernels

At the terminal type:
 ```
python -m ipykernel install --user --name pmagpy
 ```

 ## Launch Jupyterlab

Open a new terminal window. At the terminal type:
 ```
jupyter lab
 ```
You should have the option to choose `pmagpy` as a kernel for a Jupyter notebook.
