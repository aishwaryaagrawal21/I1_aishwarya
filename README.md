# Albumy

*Capture and share every wonderful moment.*

> Example application for *[Python Web Development with Flask](https://helloflask.com/en/book/1)* (《[Flask Web 开发实战](https://helloflask.com/book/1)》).

Demo: http://albumy.helloflask.com

![Screenshot](https://helloflask.com/screenshots/albumy.png)

## Installation

clone:
```
$ git clone https://github.com/greyli/albumy.git
$ cd albumy
```
create & activate virtual env then install dependency:

with venv/virtualenv + pip:
```
$ python -m venv env  # use `virtualenv env` for Python2, use `python3 ...` for Python3 on Linux & macOS
$ source env/bin/activate  # use `env\Scripts\activate` on Windows
$ pip install -r requirements.txt
```
or with Pipenv:
```
$ pipenv install --dev
$ pipenv shell
```
generate fake data then run:
```
$ flask forge
$ flask run
* Running on http://127.0.0.1:5000/
```
Test account:
* email: `admin@helloflask.com`
* password: `helloflask`


## Setting up Azure Cognitive services for the subscription key and endpoint - 

- If you haven't already, create an Azure account at https://azure.microsoft.com/en-us/free/.
- Once you have an Azure account, sign in to the Azure portal at https://portal.azure.com/.
- Click on the "Create a resource" button (+) in the left-hand menu.
- Search for "Cognitive Services" in the search box and select it from the results.
- Choose the specific cognitive service that you want to use, such as Computer Vision or Face.
- Follow the prompts to create the service. When creating the service, you will be asked to specify a name, resource group, location, - pricing tier, and subscription. You can choose the free pricing tier if you just want to try out the service.
- After creating the service, navigate to the "Keys and Endpoint" page for the service. Here you will find the subscription key and endpoint that you need to use to authenticate your requests to the API.

# Replace with your own subscription key and endpoint in the code in main.py under the 'blueprints' folder in 'albumy'. 

subscription_key = 'your-subscription-key'
endpoint = 'https://your-resource-name.cognitiveservices.azure.com/'


## License

This project is licensed under the MIT License (see the
[LICENSE](LICENSE) file for details).
# empty-aishwara21
