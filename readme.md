## Install python

Go to https://www.python.org/ to install the latest version of python for your OS

For Windows : https://www.python.org/ftp/python/3.9.6/python-3.9.6-amd64.exe

For MacOS : https://www.python.org/ftp/python/3.9.6/python-3.9.6-macosx10.9.pkg

For Linux:

sudo apt install build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libsqlite3-dev libreadline-dev libffi-dev curl libbz2-dev

wget -O https://www.python.org/ftp/python/3.9.6/Python-3.9.6.tar.xz

tar -xf Python-3.9.6.tar.xz

./configure --enable-optimizations

make -j 4

sudo make altinstall

## Setup

installing dependencie
```sh
pip3 install pipenv
```
Go inside the project folder after that type the following command
```sh
pipenv install
pipenv shell
```
## Credentials Json

There is a file call credentials.json edit that file with your twitter API info and login info.

{   

  "api_key": "your_api_key",  
  "api_secret": "your_api_secret",  
  "token_access": "your_token_access",  
  "token_secret": "your_token_secret",  
  "username": "your_username",  
  "password": "your_password"  

}

# Running the program

To populate the sql database
```sh
python3 twitter_scraper.py
```
To run the web app locally
```sh
python3 manage.py runserver
```

Visit http://127.0.0.1:8000/# Crypto-Twitter
