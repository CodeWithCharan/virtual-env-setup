# Virtual Environment Set Up

### 1. Create a virtual environment for the default version:

```
python -m venv yourenv
```

(Or)

### Create a virtual environment for the specific Python version:

```
virtualenv -p <paste_python_3.7_path_location> yourenv
```

###  2. Activate the virtual environment:

- In Command Prompt (CMD):
```
yourenv\Scripts\activate.bat
```

- In PowerShell:
```
yourenv\Scripts\Activate.ps1
```

## 3. Install ipykernel
```
pip install ipykernel
```

### 4.  Set jupyter kernel for the virtual environment

```
ipython kernel install --user --name=yourenv
```

### 5. Select the installed kernel when you want to use jupyter notebook in this virtual environment

![image](https://github.com/CodeWithCharan/virtual-env-setup/assets/106027109/aca431ae-b861-447a-97c6-08a181681fb9)

### 6. If you want to freeze your requirements (optional):
```
pip3 freeze > requirements.txt  # Python3
pip freeze > requirements.txt  # Python2
```

### 7. If you no longer need the kernel you can uninstall it (optional):

```
jupyter-kernelspec uninstall yourenv
```

