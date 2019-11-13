jupyembed
---------


Embed your data in jupyter notebooks.


* Free software: BSD license
* Documentation: https://jupyembed.readthedocs.io.


Usage
--------

Super early alpha, NOT PRODUCTION READY, NOT TESTED, WORKS FOR VANILLA CSV FILES

```
pip install jupyembed
```

Embed (multiple) data files to your notebook from the terminal using
```
jupyembed notebook.ipynb data_file.csv another_data_file.csv
```

read in data inside a notebook

```
import jupyembed
jupyembed.embed.read_embeded_data('notebook.ipynb', 'data_file.csv') # for data_file
jupyembed.embed.read_embeded_data('notebook.ipynb', 'another_data_file.csv') # for another_data_file

```

This will return a pandas dataframe by default, for a numpy array.

```
jupyembed.embed.read_embeded_data('notebook.ipynb', 'data_file.csv', dataframe=False) # will return a numpy array

```
Features
--------

* TODO

Credits
-------

This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
