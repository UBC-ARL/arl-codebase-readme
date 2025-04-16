# Qt for Python

Qt is a powerful tool to create cross-platform GUI applications. It has an official Python binding named [PySide](https://doc.qt.io/qtforpython-6). Therefore, complex GUI application development is possible with Python, and can be relatively easy to migrate to C++ Qt applications later, if performance is a concern.

> [PyQt](https://www.riverbankcomputing.com/software/pyqt/) is yet another Qt binding for Python. It is not official and may have licensing issues. In most of the cases their code are interchangeable. So if you found some example PyQt code, with minor modifications, it should work with PySide as well.

## PyQtGraph

[PyQtGraph](https://www.pyqtgraph.org/) is a pure-python graphics and GUI library built on PyQt / PySide and NumPy. When using Qt for Python, PyQtGraph provides better integration with the GUI framework than Matplotlib, in terms of signal/slot system and rich interaction.
