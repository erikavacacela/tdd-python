# Welcome to tdd with python

Examples using TDD with python.


### Prerequisites

* python3
* virtualenv [latest version](https://virtualenv.pypa.io/en/latest/)


### Manage environment

* Create a environment
```
python3 -m virtualenv env -p python3
```

* Select environment
```
source env/bin/activate
```

### Install dependencies

````
pip install spacy selenium pytest flask

pip install -e .
````


### Execute test

* Execute all test

````
python -m pytest test/test_ner_client.py
````

* Execute one test
````
python -m pytest test/test_ner_client.py::TestNerClient::test_get_ents_returns_dictionary_given_empty_string_causes_spacy_docs_ents
````







