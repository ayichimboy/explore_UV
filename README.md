# explore_UV
officially, uv has not standard mean but was developed by astreal in rust to function like pip or poetry
uv is a dependency and python library package manager. 

# Path Issues
Even after install uv, i kept getting path errors regarding uv not found after running uv --version
to correct this, I found path where uv was install locally on my computer  and using git bash, pointed python to it. 

 -- procedure
 1. pip install uv
 if uv is already installed, the path will be provided to you in the python command line 

 2. using echo, update the code to correct the path. This tells gitbash where uv.exe is found 
 echo 'export PATH="$PATH:/c/Users/Owner/AppData/Local/Packages/PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0/LocalCache/local-packages/Python311/Scripts"' >> ~/.bashrc

3. reload the shell using 
source ~/.bashrc

4. run version command to see version number of the uv installed
uv --version

5. use 
uv .venv to create virtual environment

6. use
source .venv/Scripts/Activate to activate virtual environment 

7. use 'uv add library' to add new libraries

8. add jupyterlab and ipykernel to access the kernels

9. add "uv add pip"

