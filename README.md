# Welcome to tdd with python

Examples using TDD with python.


### Prerequisites

* python3
* virtualenv [latest version](https://virtualenv.pypa.io/en/latest/)
* ChromeDriver [Chrome for Selenium](https://chromedriver.chromium.org/)


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

```
pip install spacy selenium pytest flask

pip install -e .
```


### Execute test

* Execute all test

```
python -m pytest test/test_ner_client.py
```

* Execute one test
```
python -m pytest test/test_ner_client.py::TestNerClient::test_get_ents_returns_dictionary_given_empty_string_causes_spacy_docs_ents
```


* Execute E2E test
```
python -m pytest test/test_index_e2e.py::E2ETests::test_page_has_button_for_subnitting_text
```


* Execute api test
```
python -m pytest test/test_api.py::TestApi::test_ner_endpoint_given_json_body_returns_200
```




