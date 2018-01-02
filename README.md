# My JSON Resume

## What is my JSON Resume?

It is my personal resume writen in [JSON Resume](https://jsonresume.org/). The open source initiative to create a JSON-based standard for resumes.

### Installing

#### Preferred way to install prerequisites

I prefer a virtual environment up and running and install dependencies on it. To install virtual environment we'll use Pip, which lets us install Python libraries in their own little environment that won't affect others (nor force us to install tools globally).

##### Install Pip
```bash
sudo apt-get install -y python-pip
```

##### Use Pip to install virtualenv
```bash
# -U updates it if the package is already installed
sudo pip install -U virtualenv
```

##### Create a python virtual environment
```bash
virtualenv .venv
```

##### Enable the python virtual environment
```bash
source .venv/bin/activate
```

#####  Then anything we intall with pip will be inside that virtual environment
```bash
pip install nodeenv
```

##### Create a node virtual environment
```bash
nodeenv .nenv
```

##### Activate the node virtual environment
```bash
source .nenv/bin/activate
```

#####  Then anything we intall with npm will be inside that virtual environment

###### Install the command line

The official resume-cli to run the development server.

```bash 
npm install -g resume-cli
```
