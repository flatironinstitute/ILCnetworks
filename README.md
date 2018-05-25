
# ILC regulatory network explorer

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/flatironinstitute/ILCnetworks/master)

This repository uses Jupyter notebooks and encrypted data.

You must provide a decryption key when running the `decrypt data notebook widget.ipynb` 
notebook  to
decrypt the data before viewing the regulatory network data.
After you provide the correct password to the widget in the `decrypt data notebook widget.ipynb` 
notebook the widget will explode the encrypted and compressed archive
`ILCnetworks.crypt` to create a folder `ILCnetworks`
containing notebooks and data related to ILC regulatory networks.

This repository is designed to either run in the cloud using 
[Binder](https://mybinder.org/v2/gh/flatironinstitute/ILCnetworks/master)
or locally in a encapsulated container using
[`repo2docker`](https://repo2docker.readthedocs.io/en/latest/)
to build and run a `docker` container which includes
the code for running the analysis and all needed dependencies.
The `repo2docker` tool requires the `docker` infrastructure
and Python 3 to run.  See the 
[installation instructions](https://repo2docker.readthedocs.io/en/latest/install.html).

To build and run the docker image from the command line

```bash
jupyter-repo2docker https://github.com/flatironinstitute/ILCnetworks
```
