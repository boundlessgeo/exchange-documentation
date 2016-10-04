Steps to build documents
========================

1. Create virtual environment (venv)

   `demo:boundless exchange$ virtualenv venv`

2. Activate virtual environment

   `demo:boundless exchange$ source venv/bin/activate`

3. Install Sphinx

   `(venv) demo:boundless exchange$ pip install -r requirements.txt`

4. Add submodule (theme)

   `git submodule init`
   `git submodule update`

5. build html

   `make clean html`

   Output files will be located in `build/html`

6. build wheel package for exchange

   `make clean wheel`

   Output file will be located in `build\`

7. update gh-pages

   `make clean gh-pages`

   Updated docs will be located [here] (https://boundlessgeo.github.io/exchange-documentation/).

8. push to pypi, bump patch version of python package and update patch version in github master

   `make clean pypi`

   Updated package will be located [here] (https://pypi.python.org/pypi/django-exchange-docs).
