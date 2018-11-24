## for VSCODE

* install codeLLDB plugin
* reference configuation
    ```
  {
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "type": "lldb",
            "request": "launch",
            "name": "Debug",
            "program": "${workspaceRoot}/target/debug/${workspaceRootFolderName}",
            "args": ["--dev"],
            "cwd": "${workspaceFolder}",
            "sourceLanguages": ["rust"]
        }
    ]
  }
 
* run `rm -rf ~/Library/Application\ Support/Substrate/chains/development/` if see the invalid block error
