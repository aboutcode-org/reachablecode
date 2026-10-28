=================
ReachableCode
=================

ReachableCode is a collection of pipelines for analyzing code reachability.
It integrates with ScanCode.io as a pipeline plugin
and uses tools like (Atom, CPG, .. ) to determine whether
vulnerable code symbols are reachable within a project's codebase.

Other information:

- License: Apache-2.0
- Copyright (c) nexB Inc., AboutCode.org and others.
- Homepage: https://github.com/aboutcode-org/reachablecode/
+ Documentation: https://reachablecode.readthedocs.io/

Requirements
------------

- ScanCode.io https://github.com/nexB/scancode.io

See also the next section for detailed instructions.


Local installation and usage test
------------------------------------

To install:
~~~~~~~~~~~~

- Clone reachablecode locally side-by-side: ``git clone https://github.com/aboutcode-org/reachablecode``
- Clone ScanCode.io locally side-by-side: ``git clone https://github.com/aboutcode-org/scancode.io``
- Change to the scancode.io directory and run ``make dev`` then ``source bin/activate``

  - Follow the full instructions at https://scancodeio.readthedocs.io/en/latest/installation.html#local-development-installation

- Run ``pip install --editable ../reachablecode``
- Run ScanCode.io with ``./manage.py runserver --insecure`` and open the URL in your browser.
  There is a new "analyze_atom_reachability" pipeline available when creating a new project.

Development
----------------

- Install requirements and dependencies using ``make dev``
- Then ``source venv/bin/activate``

Testing:

- To run tests: ``pytest -vvs``
