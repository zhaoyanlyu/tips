# Tips for Python basic packages and other basic utilities
+ Packages
  + sys
  + os
  + argparse
+ utility
  + Create requirements.txt


-----
## sys
### Add a working directory to the system PATH environment variable to make sure the code runs. (Solving the problem when we sometimes get an error when importing the customized packages.)
```Python
sys.path.append('PATH_TO_PROJECT_ROOT_DIR')
```

## os
### get current path
```python
os.getcwd()
```
### create path
```python
os.makedirs(path, exist_ok=Ture)
```
The ```exist_ok``` parameter prevent python from complaining about exist path.
## argparse
### Programmaly assign arguements
Sometimes we want to assign the argparse arguments programmly in stead of using command line. For the sake of looping a number of parameter choices for example. Then we can use the following Python code.
```
args = argparse.Namespace(arg1=0)
```
Note that we usually setup parser using '--arg1'. In this case, the dashes ('--') are not needed.

-----
## Create requirements.txt
```
in\the\virtualenv\ pip3 freeze > requirements.txt
```
> Ref: [stackoverflow](https://stackoverflow.com/a/33468993)
