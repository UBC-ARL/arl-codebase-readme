# Python

Python guides are everywhere. This section is not a quick-start guide for Python programming, but rather a collection of useful tips and best-practices in Python application developments.

## Installation

This section will only talk about bare Python installation. The use of [Anaconda](https://anaconda.org/) will not be discussed.

- Windows 10/11
  ```powershell
   winget install python
  ```
- MacOS
  ```bash
   brew install python
  ```
- Linux
  ```bash
   sudo apt install python3
  ```

Python is also fast changing. Some of the features mentioned in this section may not be available in older versions. This section assumes Python >=3.10.

## Virtual Environment

Dependency issues are common in Python, especially when multiple projects depend on a package but with different versions. It is recommended to use a [virtual environment](https://docs.python.org/3/library/venv.html) for each project.

## Python Package Manager

Creating a virtual environment is not enough. You also need a dependency manager to manage the packages in the virtual environment. The basic solution is to use `venv` + `pip`, with a `requirements.txt` file to list the packages. However, there are better solutions available.

This codebase by default uses [`Poetry`](https://python-poetry.org/) as the dependency manager, which manage both the virtual environment and the packages. With `Poetry`, you don't need to invoke `venv` or `pip` directly. You can use `poetry` command to manage the virtual environment and packages.

To clone and install a `Poetry` project, you can use the following command:

```bash
git clone <repo>
cd <repo>
git submodule update --init --recursive
poetry install
```

Please refer to the [Poetry documentation](https://python-poetry.org/docs/) for more information.

For projects depend on `conda` packages, consider [`pixi`](https://pixi.sh/).

## Type Hint

Refer to [typing](https://docs.python.org/3/library/typing.html).

## Handy Libraries

The reason Python is so popular is because of its rich ecosystem of libraries, which makes quick prototyping, and your life easier. This section lists some of the most commonly used libraries in Python development.

### Standard Libraries

The following libraries are part of the Python standard library. You can use them without installing any additional packages.

- [itertools](https://docs.python.org/3/library/itertools.html)
- [functools](https://docs.python.org/3/library/functools.html)
- [multiprocessing](https://docs.python.org/3/library/multiprocessing.html)
- [collections](https://docs.python.org/3/library/collections.html)
- [dataclasses](https://docs.python.org/3/library/dataclasses.html)
- [contextlib](https://docs.python.org/3/library/contextlib.html)
- [pathlib](https://docs.python.org/3/library/pathlib.html)
- [pickle](https://docs.python.org/3/library/pickle.html)
- [logging](https://docs.python.org/3/library/logging.html)
- [pytest](https://docs.pytest.org/en/latest/)

### Third-Party Libraries

- [numpy](https://numpy.org/)
- [scipy](https://www.scipy.org/)
- [sympy](https://www.sympy.org/)
- [matplotlib](https://matplotlib.org/)
- [scikit-learn](https://scikit-learn.org/stable/)
- [pandas](https://pandas.pydata.org/)
- [pydantic](https://docs.pydantic.dev/)
- [python-ranges](https://pypi.org/project/python-ranges/)
- [click](https://click.palletsprojects.com/)
