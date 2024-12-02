### Setup.md

1. Install Codeium from VSCODE Marketplace
2. Create an enviroment : python -m venv my_env
3. my_env\Scripts\activate
Code Space 
    	chmod +x ./my_env/bin/activate
   
    ./my_env/bin/activate
   
4. pip install pandas matplotlib ipykernel 
5.pip install ruff
    ruff version
    ruff check   # Lint all files in the current directory.
    ruff format  # Format all files in the current directory.
    
6. pip install jupyter matplotlib plotly
pip install quarto
7. jupyter labextension install quarto
       - Create a file , for powershell : $null > "example.qmd"
       - BASH : touch example.qmd
       - paste the following in your markdown file :
       ---
        title: "My Quarto Document"
        author: "Your Name"
        date: "Today's Date"
        format: html
        ---
       - save and then render using : quarto render example.qmd
9. Generate Requirements.txt : pip freeze > requirements.txt
10. Checkin the code to Github
11. Publish to zenodo

