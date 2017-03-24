# PyTorch Tutorials


All the tutorials are now presented as sphinx style documentation at:

## [http://pytorch.org/tutorials](http://pytorch.org/tutorials)



# Contributing

We use sphinx-gallery's [notebook styled examples](https://sphinx-gallery.readthedocs.io/en/latest/tutorials/plot_notebook.html#sphx-glr-tutorials-plot-notebook-py) to create the tutorials. Syntax is very simple. In essence, you write a slightly well formatted python file and it shows up as documentation page.

Here's how to create a new tutorial:
1. Create a notebook styled python file. If you want it executed while inserted into documentation, save the file as `your_tutorial.py`.
2. Put it in one of the beginner_source, intermediate_source, advanced_source based on the level.
2. Include it in the right TOC tree at index.rst
3. Create a thumbnail in the index file using a command like `.. galleryitem:: beginner/your_tutorial.py`. (This is a custom directive. Argument should be a full path to the python file without a slash at the beginning.) 

In case you prefer to write your tutorial in jupyter, you can use [this script](https://gist.github.com/chsasank/7218ca16f8d022e02a9c0deb94a310fe) to convert the notebook to python file. After conversion and addition to the project, please make sure the sections headings etc are in logical order.