# Installing PmagPy

## Install miniconda

## Creating a PmagPy environment from the environment.yml file

Use the terminal or an Anaconda Prompt for the following steps:

- Create the environment from the ``environment.yml`` file:

```
      conda env create -f environment.yml
```

   The first line of the ``yml`` file sets the new environment's
   name. For details see :ref:`Creating an environment file manually
   <create-env-file-manually>`.


- Activate the new environment: ``conda activate myenv``

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
   
