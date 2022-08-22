Architecture
============

Project architecture within the Cytomining repo can be understood within the context of `Data Mining <https://en.wikipedia.org/wiki/Data_mining>`_.
Various repositories within and outside of this organization are used to help accomplish related research.

Project References
------------------

The following are a list of references which relate to the content in this document.
Please note: some of these projects exist outside the Cytomining organization.

* `CellProfiler <https://github.com/CellProfiler/CellProfiler>`_
* `Pycytominer <https://github.com/cytomining/pycytominer>`_
* `Cytominer-database <https://github.com/cytomining/cytominer-database>`_
* `Cytominer-transport <https://github.com/cytomining/cytominer-transport>`_
* `Cytominer-eval <https://github.com/cytomining/cytominer-eval>`_

Project Relationships
---------------------

The following diagram is intended to provide a rough overview of how various projects interrelate.

.. mermaid::

    flowchart LR
        images[(Cell Images)]
        CellProfiler
        csv[(CSV Files)]
        DeepProfiler
        npz[(NPZ Files)]
        cytominer-database
        parquet[(Parquet Files)]
        sqlite[(SQLite File)]
        pycytominer
        pycytominer_csv[(CSV Files)]
        cytominer-eval

        images --> CellProfiler
        images --> DeepProfiler
        CellProfiler --> csv
        DeepProfiler --> npz
        csv --> cytominer-database
        cytominer-database --> sqlite
        cytominer-database --> parquet
        npz --> pycytominer
        csv --> pycytominer
        sqlite --> pycytominer
        pycytominer --> pycytominer_csv
        pycytominer_csv --> cytominer-eval

