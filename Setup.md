### Setup.md

0. Environment Update
```bash
sudo apt update #Update Package Lists
sudo apt install -y latexmk texlive texlive-latex-extra texlive-xetex #Install latexmk and TeX Live for Myst
latexmk --version
```

1. Install UV
```bash
pip install uv
```
2. Create a virtual environment and then activate it.
```bash
uv venv
#Activate the venv
source .venv/bin/activate
```
3. [Optional] Install the locked requirements
 ```bash
uv pip sync requirements.txt
```      
4. Install some typical python libraries that are needed.
 ```bash
 pip install pandas ipykernel jupyter matplotlib plotly 
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
```bash
pip install mystmd
myst --version
myst init
myst start
# ctrl + Z to stop the myst 
# to generate the pdf report : myst build 03_publication/01-article.md --pdf
``` 

7. Generate Requirements.txt 
```bash
pip freeze > requirements.txt
```

8. Checkin the code to Github
9. Make a Release
10. Try to upload the Release in Zenodo

