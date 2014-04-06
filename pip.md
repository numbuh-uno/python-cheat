Python CLI package manager.

Analogous to Ruby `gem`.

Not part of the stdlib.

Manages package dependencies.

`pip` looks by default for packages under pypi (aka the cheeseshop) located at: <https://pypi.python.org/pypi>

It is also possible to add custom servers, and even to install from source control protocols such as git directly.

Search for a package:

    pip search $pkg

Install package:

    sudo pip install $pkg

List installed packages with versions to stdout:

    pip freeze

Install packages listed on a pip file:

    pip install -r requirements.txt

Good simple way to give a requirement list for projects intended only for developers who will clone, not end users who will do `pip install`.

Install from git repo:

    sudo pip install git+git@github.com/cirosantilli/python.git@master

`.pip` files is just a newline separated list of filenames the format is exactly the same generated by pip freeze

Show all files of installed package:

    pip show -f $pkg

Uninstall package:

    sudo pip uninstall $pkg