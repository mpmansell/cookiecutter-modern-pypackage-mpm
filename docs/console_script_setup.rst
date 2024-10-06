.. _console-script-setup:


Console Script Setup
====================

Optionally, your package can include a console script using Typer (Python 3.9+).

How It Works
------------

If the 'command_line_interface' option is set to ['argparse', 'click', or 'typer'] during setup, cookiecutter will
add a file 'cli.py' in the project_slug subdirectory. An entry point is added to
pyproject.toml that points to the main function in cli.py.

Usage
-----
To use the console script in development:

.. code-block:: bash

    pip install -e projectdir

'projectdir' should be the top level project directory with the `pyproject.toml`` file

The script will be generated with output for no arguments and --help.

--help
    show help menu and exit

More Details
------------

You can read more about Argparse at:
- https://docs.python.org/3/library/argparse.html
  
- https://realpython.com/command-line-interfaces-python-argparse/
  
- https://www.cherryservers.com/blog/how-to-use-python-argparse

- https://medium.com/swlh/learning-argparse-by-example-299c3f35f2b5

You can read more about Click at:
- https://click.palletsprojects.com/en/8.1.x/

You can read more about Typer at:
- https://typer.tiangolo.com/
