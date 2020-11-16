# first_pypi_project_example
---
## Step 1: Build your packet.
1. create a directory and diretory name is your packet name
2. add a "\__init__.py\" file, it can be blank.
3. write your code on the other file and put in the directory of you create.

## Step 2: Edit setup.py information.

## Step 3: Install twine and update setuptools.
    python -m pip install --user --upgrade twine

## Step 4: Execute sdist and bdist_wheel to generate tar.gz file and wheel file.
    python setup.py sdist bdist_wheel

## Step 5: Upload project to Test-PyPi.
    python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
    python -m twine upload dist/*

## Step 6: See your project on Test-PyPi or PyPi.
<br>
<br>

## ※See your project structure.
    pip show -f package_name
### Reference:
* [打包python module 到PYPI 上](https://medium.com/%E8%B3%87%E5%B7%A5%E7%AD%86%E8%A8%98/%E6%89%93%E5%8C%85python-module-%E5%88%B0pypi-%E4%B8%8A-aef1f73e1774)
* [Packaging Python Projects](https://packaging.python.org/tutorials/packaging-projects/)
* [Packaging and distributing projects](https://packaging.python.org/guides/distributing-packages-using-setuptools/)
* [PEP 440 -- Version Identification and Dependency Specification](https://www.python.org/dev/peps/pep-0440/)
* [Classifiers](https://pypi.org/classifiers/)
* [Choose an open source license](https://choosealicense.com/)
* [Test-PyPi](https://test.pypi.org/)
* [PyPi](https://pypi.org/)
