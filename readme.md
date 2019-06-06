## This reposistory is created with learning purposes for Terraform, focusing on Terraform Null provider.

## Purpose :

- It provides a simple example of how to create Terraform Null resource.

## How to install terraform : 

- The information about installing terraform can be found on the HashiCorp website 
[here](https://learn.hashicorp.com/terraform/getting-started/install.html)

## How to use it :

- In a directory of your choice, clone the github repository :
    ```
    git clone https://github.com/martinhristov90/terraformNullProvider.git
    ```

- Change into the directory :
    ```
    cd terraformNullProvider
    ```
- Run `terraform init` to download the null provider.

- Run `terraform plan` to see what actions are going to be performed Terraform. Output should look like this :
    ```
    ------------------------------------------------------------------------

    An execution plan has been generated and is shown below.
    Resource actions are indicated with the following symbols:
      + create

    Terraform will perform the following actions:

      + null_resource.nowhere
          id: <computed>


    Plan: 1 to add, 0 to change, 0 to destroy.

    ------------------------------------------------------------------------

    Note: You didn't specify an "-out" parameter to save this plan, so Terraform
    can't guarantee that exactly these actions will be performed if
    "terraform apply" is subsequently run.
    ```

- Run `terraform apply` to create the `null_provider` . 

- In order to destroy the created resources, you can use `terraform destroy`.