### Setup.md

1.Install UV
```bash
pip install uv '''
2. pip install uv
    Create a virtual environment:
        uv venv
    Install the locked requirements
        uv pip sync requirements.txt

3. pip install pandas ipykernel jupyter
3.pip install ruff
    ruff version
    ruff check   # Lint all files in the current directory.
    ruff format  # Format all files in the current directory.
    
4. pip install quarto
5. jupyter labextension install quarto
       - Create a file , for powershell : $null > "example.qmd"
       - BASH : touch example.qmd       
       - save and then render using : quarto render example.qmd
       quarto create project manuscript 1_pdf
6. Generate Requirements.txt : pip freeze > requirements.txt


7. Checkin the code to Github

