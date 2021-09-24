# ckanext-layout

Extension to change CKAN's standard layout. In this case the block "Welcome to CKAN" is removed from the main page.


## Requirements


Compatibility with core CKAN versions:

| CKAN version    | Compatible?   |
| --------------- | ------------- |
| <2.9            | not tested    |
| 2.9             | yes           |

## Installation

To install ckanext-layout:

1. Activate your CKAN virtual environment, for example:

     . /usr/lib/ckan/default/bin/activate

2. Clone the source and install it on the virtualenv

    git clone https://gitlab.eng-softwarelabs.de/5g-testlabor/ckanext-layout.git
    cd ckanext-layout
    pip install -e .
	pip install -r requirements.txt

3. Add `layout` to the `ckan.plugins` setting in your CKAN
   config file (by default the config file is located at
   `/etc/ckan/production.ini`).

4. Restart CKAN. 

## Developer installation

To install ckanext-layout for development, activate your CKAN virtualenv and
do:

    git clone https://gitlab.eng-softwarelabs.de/5g-testlabor/ckanext-layout.git
    cd ckanext-layout
    python setup.py develop
    pip install -r dev-requirements.txt


## Tests

To run the tests, do:

    pytest --ckan-ini=test.ini


## License

[AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
