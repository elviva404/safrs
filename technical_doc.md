# SAFRS Technical Documentation

**Last updated:** 2022-01-22\
_Document generation aided by **Documatic**_

Automatic Documentation

* [Introduction](#introduction)
* [Code Overview](#code-overview)

## Introduction

This is a technical document detailing
        at a high-level
        what SAFRS does, how it operates,
        and how it is built.

The outline of this document was generated
        by **Documatic**.
<!---Documatic-section-group: arch-start--->


## Project Architecture


<!---Documatic-section-group: arch-end--->

<!---Documatic-section-group: helloworld-start--->


## Code Overview

The codebase has a 5-deep folder structure, with 70 in total.
<!---Documatic-section-helloworld: setup-start--->
The codebase is compatible with Python 3.9 and above, because of pipe dictionary union in safrs/expose_existing/sqlacodegen/.eggs/setuptools_scm-2.1.0-py3.5.egg/setuptools_scm/win_py31_compat.py.
Install requirements with `pip install -r requirements.txt`.

Run `pip install -e .` in top-level directory to install
package in local directory.
Install from pypi with `pip install main`.



<!---Documatic-section-helloworld: setup-end--->
`safrs.examples.mini_app`` has a `__main__` entrypoint.

`safrs.examples.demo_devto`` has a `__main__` entrypoint.

`safrs.examples.demo_pythonanywhere_com` has a `__main__` entrypoint, which calls:

* `safrs.examples.demo_pythonanywhere_com.start_api`

`safrs.examples.demo_stateless`` has a `__main__` entrypoint.

`safrs.examples.demo_http_get`` has a `__main__` entrypoint.

`safrs.examples.demo_rel2` has a `__main__` entrypoint, which calls:

* `safrs.examples.demo_rel2.start_api`

`safrs.examples.demo_relationship`` has a `__main__` entrypoint.

`safrs.examples.demo_flaskrestjsonapi`` has a `__main__` entrypoint.

`safrs.examples.demo_geoalchemy` has a `__main__` entrypoint, which calls:

* `safrs.examples.demo_geoalchemy.connect_to_db`

`safrs.examples.demo_full` has a `__main__` entrypoint, which calls:

* `safrs.examples.demo_full.start_api`

`safrs.expose_existing.expose_existing` has a `__main__` entrypoint, which calls:

* `safrs.expose_existing.expose_existing.start_api`


<!---Documatic-section-helloworld: entrypoints-start--->


## Entrypoints

There are 0 source code entrypoints in top-level `__main__`/`__init__` files.


<!---Documatic-section-helloworld: entrypoints-end--->

<!---Documatic-section-group: concept-start--->
## Concepts
<!---Documatic-section-group: concept-end--->

<!---Documatic-section-group: helloworld-end--->

<!---Documatic-section-group: dev-start--->


## Developers
<!---Documatic-section-dev: setup-start--->
* Tests are present in `tests/`




<!---Documatic-section-dev: setup-end--->

<!---Documatic-section-dev: ci-start--->
The project uses GitHub Actions for CI/CD.

| CI File | Purpose |
|:----|:----|
| codeql-analysis |  |
| python-app |  |


<!---Documatic-section-dev: ci-end--->

<!---Documatic-section-group: dev-end--->

### **safrs/**

#### swagger-editor/

##### test/

###### e2e/

###### tests/

No files in `tests/` import local package files.

##### docs/

No files in `docs/` import local package files.

#### tests/

No files in `tests/` import local package files.

#### docs/

No files in `docs/` import local package files.

#### safrs/

No files in `safrs/` import local package files.

<!---Documatic-section-file: safrs/safrs_api.py--->

### safrs_api.py


File has 59 lines added and 6 lines removed
                in the past 4 weeks. Thomas Pollet <thomas.pollet@gmail.com> is the inferred code owner.


<!---Documatic-section-file: safrs/jsonapi_formatting.py--->

### jsonapi_formatting.py


File has 37 lines added and 36 lines removed
                in the past 4 weeks. Thomas Pollet <thomas.pollet@gmail.com> is the inferred code owner.


<!---Documatic-section-file: safrs/base.py--->

### base.py


File has 11 lines added and 12 lines removed
                in the past 4 weeks. Thomas Pollet <thomas.pollet@gmail.com> is the inferred code owner.


#### examples/

`examples/` relies most on `safrs/` (imports 85 times).

#### expose_existing/

`expose_existing/` relies most on `safrs/` (imports 5 times).

###### sqlacodegen/

###### tests/

No files in `tests/` import local package files.