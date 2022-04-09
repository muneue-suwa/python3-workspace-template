# Python3 Workspace Template

This is Visual Studio Code Workspace Template for Python3.

## Settings File

You can download directly settings.json from [this link](https://raw.githubusercontent.com/muneue-suwa/python3-workspace-template/master/.vscode/settings.json).

### Windowns

1. Create `.vscode/`.

  ```powershell:create-dot-vscode-dir
  New-Item .vscode -ItemType Directory
  ```

2. Download and save the settings file.

  ```powershell:download-settings-json
  Invoke-WebRequest -Uri https://raw.githubusercontent.com/muneue-suwa/python3-workspace-template/master/.vscode/settings.json -OutFile .vscode/settings.json
  ```

## Reference

[VS Code コーディング規約を快適に守る](https://qiita.com/firedfly/items/00c34018581c6cec9b84)
