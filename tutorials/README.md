# Tutorials

This directory contains all of the tutorials for selene.

The most thorough tutorial for getting started is in [`getting_started_with_selene`](https://github.com/FunctionLab/selene/tree/master/tutorials/getting_started_with_selene).
To get started on training a model very quickly, please see [`quickstart_training`](https://github.com/FunctionLab/selene/tree/master/tutorials/quickstart_training).

Additionally, we have two tutorials that show how to apply trained models. Selene provides methods to run variant effect prediction and _in silico_ mutagenesis, along with some visualization methods that we recommend running based on our Jupyter notebook tutorials.

- Comprehensive _in silico_ mutagenesis tutorial: [`analyzing_mutations_with_trained_models`](https://github.com/FunctionLab/selene/tree/master/tutorials/analyzing_mutations_with_trained_models)
- Tutorial with both the config file method and the non-config file method of running Selene. Also shows how to run variant effect prediction and visualize the difference scores. Contains an _in silico_ mutagenesis example with known regulatory mutations: [`variants_and_visualizations`](https://github.com/FunctionLab/selene/tree/master/tutorials/variants_and_visualizations) 

## Contributing tutorials

The process for adding a tutorial to selene is as follows:

1. Create a subdirectory in the tutorials directory. The name of this subdirectory should be the name of the tutorial, formatted in snake-case.
2. Write the tutorial in an [ipython notebook](https://ipython.org/notebook.html) in the subdirectory.
3. Store all data for the tutorial in the subdirectory, and create a gzipped archive (i.e. a `*.tar.gz` file) with all the data required for the tutorial.
4. Create a `*.nblink` link file in the `docs/source/tutorials` directory. This file will serve as a link to the tutorial's notebook file. Instructions for formatting this file can be found [here](https://github.com/vidartf/nbsphinx-link).
5. Add an entry for the tutorial to the list of tutorials in `docs/source/tutorials/index.rst`.
6. Rerun `make html` from the `docs` directory.

