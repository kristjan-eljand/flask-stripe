# flask-stripe
Flask and Stripe for handling subscriptions

# Environment setup
**Test if you have python 3.9 or higher**
* `python3 -V`

**If you have older version, install python 3.9 (Linux 18.04 & 20.04)**
* `sudo apt-get update`
* `sudo apt install software-properties-common`
* `sudo add-apt-repository ppa:deadsnakes/ppa`
* `sudo apt-get install python3.9`

Add both old and new version of python to update alternatives.
* `sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.[your-old-version] 1`
* `sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9 2`

Type this command to set the new python version as a default one:
* `sudo update-alternatives --config python3`
The command line prompt will now ask you to select your version -> select the new installation version number.

Check the python version again to see if the upgrade was successful
* `python3 -V`

**Install virtualenv package**
* `sudo apt-get install virtualenv`

**Clone the code repository and go to its main directory**
* `git clone git@github.com:kristjan-eljand/flask-stripe.git`
* `cd flask-stripe`

**Create virtualenv named venv and activate it**
* `virtualenv -p python3.9 venv`
* `source venv/bin/activate`

**Install requirements file**
* `pip install -r requirements.txt`

# Run the app
* `export FLASK_APP=myapp`
* `export FLASK_ENV=development`
* `flask run`
