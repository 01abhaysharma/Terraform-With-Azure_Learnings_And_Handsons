# Terraform Basic Commands

1. **Checking Terraform Version**

    As a first step, you must check the version of Terraform you are currently running. You can do this by running the following command in your terminal:

    ```bash
    terraform -v
    ```

2. **Initializing Terraform Project**

    The `terraform init` command is an essential first step in any Terraform project. It initializes your working directory according to the code in your Terraform files. It also downloads the necessary providers for your infrastructure. Run the following command to initialize your project:

    ```bash
    terraform init
    ```

3. **Validating Terraform Configuration**

    The `terraform validate` command is used to ensure that your Terraform configuration is syntactically correct and internally consistent. It's like a grammar check for your infrastructure code. Run this command to validate your configuration:

    ```bash
    terraform validate
    ```

4. **Planning Infrastructure Changes**

    The `terraform plan` command gives you an overview of the changes your configuration will make to your infrastructure before actually applying these changes. It is like a blueprint for your infrastructure modifications. Here's how you can run it:

    ```bash
    terraform plan
    ```

5. **Applying Terraform Configuration**

    Once you’re satisfied with your plan, you can use the `terraform apply` command to apply your configuration and deploy it into your cloud provider, such as Azure:

    ```bash
    terraform apply
    ```

6. **Destroying Terraform Infrastructure**

    The `terraform destroy` command removes your deployed configuration and associated resources. Once you run this command and it completes successfully, it will destroy the resources in your cloud provider:

    ```bash
    terraform destroy
    ```

7. **Formatting Terraform Code**

    `terraform fmt` (short for format) command helps you maintain clean and readable code. It reformats your code to align with HashiCorp Language (HCL) standards. Run this command to format your current directory:

    ```bash
    terraform fmt
    ```
