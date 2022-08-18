# Python3 Workspace Template

This is Visual Studio Code Workspace Template for Python3.

## How to use this template

Click `Use this template` from GitHub or download directly settings.json from [this link](https://raw.githubusercontent.com/muneue-suwa/python3-workspace-template/master/.vscode/settings.json).

### How to download directly settings.json

### Windows

  ```powershell
  New-Item .vscode -ItemType Directory
  Invoke-WebRequest -Uri https://raw.githubusercontent.com/muneue-suwa/python3-workspace-template/master/.vscode/settings.json -OutFile .vscode/settings.json
  ```
### Linux

  ```bash
  mkdir .vscode
  wget https://raw.githubusercontent.com/muneue-suwa/python3-workspace-template/master/.vscode/settings.json -O .vscode/settings.json
  ```

## Virtual Environment

Install Python virtual environment and select the interpreter from VSCode Command Palette (`Ctrl+Shift+P`)

### Windows

```powershell
python -m venv .env
.env\Scripts\activate  # (.env) will be shown
pip install -U pip
# And then Select Python Interpreter from VSCode Command Palette
```

If you use python virtual environment **for the first time**, execute the following command.

```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```
### Linux

```bash
python -m venv .env
source .env/bin/activate  # (.env) will be shown
pip install -U pip
# And then Select Python Interpreter from VSCode Command Palette
```

## requirement.txt

### Windows

```bash
pip install -r requirements.txt  # Install third-party libraries from requirements.txt
pip freeze | Out-File -Encoding UTF8NoBOM requirements.txt  # Export libraries list to requirement.txt
```

### Linux

```bash
pip install -r requirements.txt  # Install third-party libraries from requirements.txt
pip freeze > requirements.txt  # Export libraries list to requirement.txt
```

## Reference

[VS Code コーディング規約を快適に守る](https://qiita.com/firedfly/items/00c34018581c6cec9b84)
