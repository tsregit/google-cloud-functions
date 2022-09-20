# Google Cloud Functions
## Starting a project

To start a new project in Google Cloud, we can go to the [Firebase Console](https://console.firebase.google.com) or create it from [Google Cloud Platform Console](https://console.cloud.google.com)

## Creating a virtual environment
First we have to install `python3-venv` with the following command

**Linux**
```
sudo apt install python3-venv
```
**Homebrew**
```
brew install virtualenv
```
**Command for created a new virtual environment**
```
python3 -m venv venv
```
**To activate the virtual environment we do**
```
source venv/bin/activate
```
In order to add new packages to our new virtual environment we create a file called `requirements.txt` and execute the following 
```
pip install -r requirements.txt
```

## Deploying our functions
First, we have to set put project ID with the following commando:
```
gcloud config set project [PROJECT_ID]
```
Then we deploy pur function with this command:
```
gcloud functions deploy [FUNCTION_NAME] --runtime python37 --trigger-http
```
