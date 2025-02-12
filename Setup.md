### Setup.md

1. Install UV
```bash
pip install uv
```
2. Create a virtual environment
```bash
uv venv
```
3. [Optional] Install the locked requirements
 ```bash
uv pip sync requirements.txt
```      
4. Install some typical python libraries that are needed.
 ```bash
 pip install pandas ipykernel jupyter matplotlib plotly jupyterlab-magic-wand
```
5. Install Ruff
```bash
pip install ruff
ruff version
ruff check   # Lint all files in the current directory.
ruff format  # Format all files in the current directory.
# ruff check --fix
```
6. ### Install MyST
* Install Myst(https://mystmd.org/guide/installing), https://mystmd.org/guide/quickstart-myst-documents

At the terminal type:  
```
pip install mystmd
myst --version
myst start
``` 

7. Generate Requirements.txt : pip freeze > requirements.txt

8. Checkin the code to Github
9. Make a Release
10. Try to upload the Release in Zenodo

