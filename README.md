# Hydrology Thematic Exploitation Platform Documentation

This is the official repository of Hydrology Thematic Exploitation Platform Documentation. This
documentation is live at:
[http://hydrology-tep.github.io/documentation](http://hydrology-tep.github.io/documentation).

You are encouraged to fork this repo and send us pull requests!

## Getting started

Here's the procedure to install the required packages on a CentOS 6.x

```
sudo yum install python-sphinx
sudo yum install python-pip
```

As root do:

```
pip install sphinx_bootstrap_theme
```

Back as your user, do:

```
git clone git@github.com:hydrology-tep/documentation.git
cd documentation
```

If needed, set your github information

```
git config --global user.name <github username>
git config --global user.email <email address>
```

## Building

Build the documentation by running ``make html``.

## Publish the documentation

``make html`` creates a ``build`` folder in the *documentation* local repository.

As root, do:

```
cd /var/www/html
ln -s $HOME/documentation/build/html/ documentation
chown apache:apache documentation
```

Open you browser at the address http://127.0.0.1/documentation

## This documentation is built with sphinx-doc

[More information](http://sphinx-doc.org/).
