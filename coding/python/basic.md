# Tips for Python basic packages.
+ sys
+ os

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
