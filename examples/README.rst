Examples
========

This gallery contains a selection of examples of the plots mplsoccer can create.

All of the examples can be run from the following Anaconda environment:

   .. code :: yaml

      name: mplsoccer
      channels:
        - anaconda
        - conda-forge
      dependencies:
        - jupyter
        - pandas
        - scipy
        - seaborn
        - beautifulsoup4
        - pyarrow
        - conda-forge::ffmpeg
        - pip
        - pip:
            - mplsoccer

To install the environment yourself use the `Anaconda <https://www.anaconda.com/>`_ Prompt:

#. Copy the code above into a blank file called ``environment.yml``, then run the following command from the directory containing the file.

   .. code ::

      conda env create -f environment.yml

#. Activate the new environment:

   .. code ::

      conda activate mplsoccer
      