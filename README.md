https://realpython.com/python-project-documentation-with-mkdocs/

cd "Users\BilalBobat\OneDrive - Flagstone\Python"

mkdir mkdocs-documentation
cd mkdocs-documentation

python -m venv venv
venv\Scripts\activate

python -m pip install mkdocs
python -m pip install "mkdocstrings[python]"
python -m pip install mkdocs-material

python -m pip list

pip freeze > requirements.txt

mkdir calculator

cd calculator

New-Item -Path "calculations.py" -ItemType File
New-Item -Path "calculations.py" -ItemType File

## alternative option
echo > __init__.py
echo > calculations.py

python -m doctest calculator\calculations.py

venv\Scripts\activate

mkdocs new .

mkdocs serve

venv/scripts/activate
mkdocs serve
git checkout -b main
git init
git remote add origin https://github.com/bilalbobat/calculator.git

git push -u origin main

git branch -m master main
git checkout -b main

git add .
git commit -m "Initial commit"
git push -u origin main

mkdocs gh-deploy

https://bilalbobat.github.io/calculator/