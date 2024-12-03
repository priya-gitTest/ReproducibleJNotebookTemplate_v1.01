### Setup.md

1.Install UV
```bash
pip install uv
```
2. Create a virtual environment
```bash
uv venv
```
3. [Optional]Install the locked requirements
 ```bash
uv pip sync requirements.txt
```      
4. Install some typical python libraries that are needed.
 ```bash
   pip install pandas ipykernel jupyter
```
5. Install Ruff
```bash
pip install ruff
ruff version
ruff check   # Lint all files in the current directory.
ruff format  # Format all files in the current directory.
```
6. Install Quarto
```bash
   pip install quarto
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

