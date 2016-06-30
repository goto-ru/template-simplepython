Contributing
------------

Basic workflow
==============

.. code:: sh

        git clone $project
        cd $project

        # create and activate a development environment
        virtualenv -p python3.5 devenv
        source devenv/bin/activate

        # install development dependencies
        pip install -r requirements-dev.txt

        # install pre-commit hooks
        pre-commit install

        # switch to feature branch
        git checkout -b dev-$feat

        # make some changes
        $EDITOR $filename.py

        git add $filename.py
        # pre-commit hooks with linters and formatters will be run
        git commit
