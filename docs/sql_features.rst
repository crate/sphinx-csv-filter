============
SQL features
============

A real-world example from the CrateDB repository.

Sources
=======
- `compliance.rst`_
- `sql_features.tsv`_

Build
=====
::

    rm -rf out && python -m sphinx --fail-on-warning --builder html docs out

Demo
====
.. csv-filter::
   :header: ID,Package,#,Description,Supported,Verified,Comments
   :widths: 80,140,15,250,130
   :delim: U+0009
   :file: sql_features.tsv
   :exclude: {4: r'(?i)N\w*'}
   :included_cols: 0,1,2,3,6


.. _compliance.rst: https://github.com/crate/crate/blob/master/docs/appendices/compliance.rst
.. _sql_features.tsv: https://github.com/crate/crate/blob/master/server/src/main/resources/sql_features.tsv
