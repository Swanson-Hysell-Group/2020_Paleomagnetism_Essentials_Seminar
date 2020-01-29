# Installing PmagPy

## Install miniconda

Creating an environment from an environment.yml file
====================================================

Use the terminal or an Anaconda Prompt for the following steps:

#. Create the environment from the ``environment.yml`` file:

   .. code::

      conda env create -f environment.yml

   The first line of the ``yml`` file sets the new environment's
   name. For details see :ref:`Creating an environment file manually
   <create-env-file-manually>`.


#. Activate the new environment: ``conda activate myenv``

#. Verify that the new environment was installed correctly:

   .. code::

      conda env list

  You can also use ``conda info --envs``.
