### Setup.md

1. Environment Update
```bash
sudo apt update #Update Package Lists
sudo apt install -y latexmk texlive texlive-latex-extra texlive-xetex #Install latexmk and TeX Live for Myst
latexmk --version # Latexmk, John Collins, 26 Dec. 2019. Version 4.67
```

2. Install UV
```bash
pip install uv
```
3. Create a virtual environment and then activate it.
```bash
uv init # Creates a new or initialize the current directory and generates following files :  pyproject.toml, README.md, .python-version, main.py
#Another example : uv venv --python=3.12 .venv
uv venv # creates a new virtual environment for isolating Python packages and dependencies.
#Activate the venv
source .venv/bin/activate
```
3. [Optional] Install the locked requirements
 ```bash
#uv pip sync requirements.txt
#uv sync # run this to install what is present in your lock file exactly 
#uv lock # generated automaticall the first time you run uv add, uv remove or uv sync
#uv.lock file : The lockfile ensures reproducible builds by recording the exact versions of all dependencies that were resolved. 
```      
4. Install some typical python libraries that are needed.
 ```bash
 #pip install pandas ipykernel jupyter matplotlib plotly 
 uv add pandas ipykernel jupyter matplotlib seaborn groq
```
5. Install Ruff
```bash
#pip install ruff
uv tool install ruff
ruff version
ruff check   # Lint all files in the current directory. or specify a file name to check for that file.
ruff format  # Format all files in the current directory.
# ruff check --fix
```
6. ### Run your Jupyter Notebook
    - Install the following extensions  : Python [Microsoft microsoft.com]
    - Install the following extensions  : Jupyter [Microsoft microsoft.com]   
    - Choose the Global Python Environment 
    - Run the cells and play around with the prompts.

7. ### Install MyST
* Install Myst(https://mystmd.org/guide/installing), https://mystmd.org/guide/quickstart-myst-documents

At the terminal type:  
```bash
#pip install mystmd
uv tool install mystmd
myst --version
myst init
myst start
# ctrl + Z to stop the myst 
# Install a PDF viewer : PDF Viewer [Mathematic Inc]
# to generate the pdf report : myst build 03_publication/01-article.md --pdf --output 03_publication/01-article.pdf
``` 

8. Generate uv.lock file or alternatively Requirements.txt 
```bash
#pip freeze > requirements.txt
# uv pip freeze > requirements.txt
uv lock
```

9. Checkin the code to Github
10. Make a Release
    - Open the Releases Page
    - Click on "Draft a new release"
    - Choose the appropriate target branch
    - Choose a Tag Version else GitHub will create it.
    - Add a Release Title & Description
    - Click "Publish Release"
11. Try to upload the Release in Zenodo
     - Follow the steps mentioned here : https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content

