# Ktirio Urban Building AI HPDA code 

## Setup Environment

To start, you need to install the following tools:

```
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

The previous commands will create a virtual environment and install the required packages including the hid-ai-hpda-ub package.
Once the installation is done, you can start using the package or run the notebooks in `src/notebooks/`.

## Visual Studio Code

In order to use Visual Studio Code, you need to install the following extensions:

* Python
* CMake
* Docker
* Jupyter
* AI Code

We have configured `.vscode/extensions.json` to automatically install recommended extensions when you open the project in Visual Studio Code.

## Feel++ Template Project 

This repository provides a basic starting point for a Feel++ application including:

* [x] Feel++ applications in C++ to use Feel++ and Feel++ toolboxes in `src`
* [x] documentation using asciidoc and antora
* [x] continuous integration including tests for the C++ applications
* [x] docker image generation for the project
* [x] notebooks are in src/notebooks

The documentation for hid-ai-hpda-ub is available at [here](https://feelpp.github.io/hid-ai-hpda-ub) and you can build on it for your project by enabling the [github pages](https://docs.github.com/en/pages) for your repository.

## Updating the hid-ai-hpda-ub  version

The version of the project is defined in the files `CMakeLists.txt`, `docs/antora.yml`, `pyproject.toml` and `package.json`. 
You need to update with the same version in all files.

## Release process

* [x] update the version in CMakeLists.txt
* [x] update the version in docs/antora.yml
* [x] update the version in package.json
* [x] commit the version in pyproject.toml
* [x] commit the changes with the message "Release vx.y.z". At this point the CI will generate the docker image and push it to docker hub

## Team

* Christophe Prud’homme &lt;@prudhomm>
* Javier Cladellas &lt;@JavierCladellas>
* ...
