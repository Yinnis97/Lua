# Running Lua in Visual Studio Code

## Step 1 : Install Lua Extension for VSCode

1. Open VSCode.

2. Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or by pressing Ctrl+Shift+X.

3. Search for "Lua" and install the extension provided by sumneko.

## Step 2 : Configure VSCode to Run Lua Code

1. Open the Command Palette by pressing Ctrl+Shift+P.

2. Type "Tasks: Configure Task" and select it.

3. Choose "Create tasks.json file from template" and select "Others".

4. Replace the content of the tasks.json file with the following configuration:
    ```bash
    {   
        "version": "2.0.0", 
        "tasks": [  
        {   
        "label": "Run Lua", 
        "type": "shell",    
        "command": "lua",   
        "args": [   
        "${file}"   
        ],  
        "group": {  
        "kind": "build",    
        "isDefault": true   
        },  
        "problemMatcher": []    
        }   
        ]   
    }   
    ```
**This configuration tells VSCode to use the lua command to run the currently open file.**

## Step 3 : Running Lua Code

1. Open a Lua file or create a new one with the .lua extension.

2. Write your Lua code. For example:
    ```bash
        print("Hello, World!")
    ```
3. Save the file.

4. To run the Lua script, press Ctrl+Shift+B or go to the Terminal menu and select "Run Build Task".

**Your Lua code should now execute, and you should see the output in the terminal window within VSCode.**