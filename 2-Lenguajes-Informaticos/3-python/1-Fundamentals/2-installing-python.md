# Installing Python



## Installing Python on Deb systems

To install python first we need to know which version is available. We can find out which version is the newest one in the official page. https://www.python.org/downloads/



### Installation

Then we can proceed with the installation. To install it we just have to use the following command on the terminal.

```bash
sudo apt install python3.10 #newest python version
```



### Creating a file

After the installation to start using python we need to create a ".py" file .

```bash
nvim python-file.py
```



### Executing the file

To execute a python file there are two ways. The easiest  way is to write python3 and the name of the file.

```bash
python3 python-file.py
```



Another way is to give execution permissions to the file .

```bash
#Adding execute permission
chmod +x python-file.py
```

After that, inside the python file we are going to give the address to execute.

```python
 #!/usr/bin/env python3
    
 #Some python code
```

and finally we can execute the program from the terminal.

```bash
./python-file.py
```



