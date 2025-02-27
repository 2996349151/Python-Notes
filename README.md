# Python-Notes

## Project Initiallization (in Github and Visual Studio Code)

### Step 1: Create a repository on github and clone it to local 

### Step 2: Create and activate vitual environemnt
1. Open terminal by pressing <kbd>Ctrl</kbd>+<kbd>`</kbd>
2. Then create and active the virtual environemnt: 
```Bash
# Create
python3 -m venv venv
# Activate (remember activating eveytime)
source venv/bin/activate
```
3. Create a file named <kbd>.gitignore</kbd>
4. Write following codes to ignore venv when using git
```
venv/
```

### Step 3: Select interpreter
1. Open the Command Palette by pressing <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd>
2. Type <kbd>Python: Select Interpreter</kbd> and press <kbd>Enter</kbd>
3. From the list, choose the interpreter located within the virtual environment 

### Step 4: Install packages
```Bash
# Create or syncronize packages information
pip freeze > requirements.txt

# Install sepecific packages
pip install package-name

# Install all packages in requirements
pip install -r requirements.txt
```

### Step 5: Manage formatting (for Python files)
1. Install any formatter (this time is Black)
```Bash
pip install black
```
2. Create a file named <kbd>pyprojects.toml</kbd>
3. Create formatting ruls in that file, such as:
```
[tool.Black]
line-length = 88
```
4. Then format all Python files:
```Bash
Black .
```