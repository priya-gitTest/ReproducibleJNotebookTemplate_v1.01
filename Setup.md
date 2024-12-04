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
 pip install pandas ipykernel jupyter matplotlib plotly
```
5. Install Ruff
```bash
pip install ruff
ruff version
ruff check   # Lint all files in the current directory.
ruff format  # Format all files in the current directory.
```
6. ### Install the Quarto CLI
* Install the Quarto CLI. ([Quarto instructions for Linux installation](https://quarto.org/docs/download/tarball.html) which we need to do on Codespaces. If you're working locally you can download the CLI and install it.)

At the terminal type:  
`wget https://github.com/quarto-dev/quarto-cli/releases/download/v1.5.57/quarto-1.5.57-linux-amd64.tar.gz`  
`mkdir ~/opt`  
`tar -C ~/opt -xvzf quarto-1.5.57-linux-amd64.tar.gz`  
`ln -s ~/opt/quarto-1.5.57/bin/quarto ~/.local/bin/quarto`  
`quarto -v` 

### Install some VSCode extensions
* Search for the Quarto extension and install that extension
* Search for the Preview extension and install that extension
  
7. Install Quarto
```bash
pip install quarto
quarto check # Use quarto check to confirm that the installation is successful
```
8.  Render a Quarto Document     
```bash
quarto render hello.qmd
```
9. Create a Manuscript Project
```bash
quarto create project manuscript 1_pdf
```
9. Generate Requirements.txt : pip freeze > requirements.txt

10. Checkin the code to Github
11. Make a Release
12. Try to upload the Release in Zenodo

