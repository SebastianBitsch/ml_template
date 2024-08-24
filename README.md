# python machine learning / deep learning template
Install 
---
Bare bones, no junk.

Stolen from [cookiecutter-data-science](https://github.com/drivendata/cookiecutter-data-science) template.

## Requirements to use the template:

* Python 3.11
* Cookiecutter v2.4.0

## Start a new project

Start by creating a repository either using the Github GUI in the webbrowser or alternatively you can use the
[Github command line interface](https://cli.github.com/) if you have set it up:

```bash
gh repo create <repo_name> --public --confirm
```
Afterwards on your local machine run

```bash
cookiecutter https://github.com/sebastianbitsch/ml_template
```

and input starting values for the project. When asked for the repository name when creating the template,
input the same name as when you created the repository. Note that when asked for the project name, you should input
a [valid Python package name](https://peps.python.org/pep-0008/#package-and-module-names). This means that the name 
should be all lowercase and only contain letters, numbers and underscores. The project name will be used as the name of 
the Python package. This will automatically be validated by the template.

To commit to the remote repository afterwards execute the following set of commands:

```bash
cd <repo_name>
git init
git add .
git commit -m "init cookiecutter project"
git remote add origin https://github.com/<username>/<repo_name>
git push origin master
```