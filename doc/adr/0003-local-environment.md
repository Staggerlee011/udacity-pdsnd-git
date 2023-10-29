# 3. local environment

Date: 2023-10-29

## Status

Accepted

## Context

There is a need to ensure that the local environment is consistent across the team.

## Decision

To use pyenv to manage the python version and virtualenv to manage the python environment.

### local set up

- ensure you are using python 3.10 (not tested on other versions)

``` bash
pyenv install 3.10.0
```

- create a virtual environment

``` bash
python -m venv venv
```

- activate the virtual environment

``` bash
source venv/bin/activate
```

- install the dependencies

``` bash
pip install -r requirements.txt
```

## Consequences

- The local environment is consistent across the team.
- The local environment is consistent with the CI environment.
