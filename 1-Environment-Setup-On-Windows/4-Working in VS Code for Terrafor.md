# Using VS Code to work with Terraform 

1. **Install the Terraform Extension:** 

   - Open Visual Studio Code.
   - Click on the Extensions view icon on the Sidebar or press `Ctrl+Shift+X`.
   - In the Extensions search bar, type "Terraform" and press `Enter`.
   - Look for the Terraform extension published by HashiCorp and click on the 'Install' button.

    > This extension provides syntax highlighting, autocompletion, and other features that make it easier to write Terraform configuration.

2. **Create a new Terraform file:** 

   - Click on the Explorer icon on the Sidebar.
   - In the Explorer panel, navigate to the directory where you want to create your Terraform configuration file.
   - Click on the 'New File' button.
   - Name your file with a `.tf` extension (e.g., `main.tf`). This signals to VS Code that this is a Terraform configuration file.

3. **Write Terraform Configuration:** 

   - In the new `.tf` file, you can now start writing your Terraform configuration. Here's a simple example:

     ```terraform
     provider "azurerm" {
       features {}
     }

     resource "azurerm_resource_group" "example" {
       name     = "example-resources"
       location = "West Europe"
     }
     ```

     This configuration specifies a provider (in this case, Azure) and a single resource (a resource group).

4. **Open PowerShell in VS Code:**

   - Open Visual Studio Code.
   - Click on the 'Terminal' menu item at the top of the screen.
   - Click on 'New Terminal' or 'New Integrated Terminal'. This will open a new terminal at the bottom of the window. Alternatively, you can use the shortcut `Ctrl+`` (the backtick key, which is usually located below the `Esc` key).
   
   > By default, the terminal will open with PowerShell as the shell in a Windows environment. If it's not PowerShell, you can change it: 
     - Click on the 'Terminal' menu item at the top of the screen.
     - Click on 'Select Default Shell'.
     - Select 'Windows PowerShell' from the dropdown menu.

    From now on, every new terminal you open in VS Code will use PowerShell by default. You can always change this setting later if you need to use a different shell.

   > Remember to save your file (`Ctrl+S`) after making changes. The Terraform extension in VS Code provides real-time feedback and will highlight any syntax errors in your configuration. You can also use the built-in terminal in VS Code to run Terraform commands directly.

