# ePages Beyond Example Payment App

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/ooz/epages-beyond-payment-app/tree/master)

Test payment app for development purposes. Provides simple mock responses to requests.

## Dependencies

- [Python3](https://www.python.org/downloads/)
- [pip](https://pypi.org/project/pip/)
- [Pipenv](https://pipenv.pypa.io/en/latest/)
- [Make](https://en.wikipedia.org/wiki/Make_(software))

**Ubuntu**

If you are using Ubuntu as operating system, follow those steps to install the dependencies:

```bash
sudo apt update
sudo apt install python3-pip make
sudo pip3 install pipenv
pipenv --three install --dev
```

## Development

### Run tests

Before you can run the tests, you need to provide the client ID and client secret of the app:

```bash
cp pytest.ini.template pytest.ini
vim pytest.ini
```

Then you can run the tests by calling the `test` task:

```bash
make test
```
