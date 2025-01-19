# How to Install Lua on Windows 10/11
**Follow these steps to install Lua on your Windows system:**

## Step 1: Download the Required Files

1. Download LuaBinaries:    
Visit [LuaBinaries](https://luabinaries.sourceforge.net/)
and download the latest version suitable for your system (32-bit or 64-bit).

2. Download LuaDist:    
Go to [LuaDist](https://luadist.org/repository/) Repository and download the package management system for windows.

## Step 2: Unzip and Combine the Files

1. Extract both LuaBinaries and LuaDist files using an unzip tool (e.g., WinRAR, 7-Zip, or the built-in Windows utility).
2. Create a folder named Lua in the root of your C: drive (e.g., C:\Lua).
3. Copy all the content from both extracted folders into this Lua folder.

## Step 3: Add Lua to System Environment Variables
To make Lua accessible from anywhere in the command line:

1. Press **Windows + R**, type **sysdm.cpl**, and hit Enter.
2. In the **System Properties** window, go to the **Advanced tab** and click **Environment Variables**.
3. Under **User variables**, locate and select the variable named **Path**. Then, click Edit.
4. In the **Edit Environment Variable** window, click **New**, and paste the path to Lua's bin folder: **C:\Lua\bin**
5. Click OK to save your changes, and close all dialog boxes.

## Step 4: Verify the Installation

1. Open a Command Prompt.    
2. Type lua and hit Enter.  
3. If Lua is installed correctly, you'll see the Lua version and the Lua interactive shell prompt (e.g., >).    
4. If you don't see this, double-check the installation steps and ensure the Path variable is correctly set.        

## Additional Tips

- Save your Lua scripts with the .lua extension and run them in the command prompt using the lua <filename>.lua command.  
- Refer to the official Lua documentation at Lua.org for further guidance and learning resources.

## Sources

- [LuaBinaries](https://luabinaries.sourceforge.net/)
- [LuaDist](https://luadist.org/repository/)
- [YouTube Tutorial](https://www.youtube.com/watch?v=zXW7YqoMUpA)
