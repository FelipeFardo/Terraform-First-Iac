# Terraform-First-Iac

This project demonstrates the use of Infrastructure as Code (IaC) with Terraform to provision AWS resources. It serves as a starting point for those looking to automate infrastructure in a declarative and reproducible way.

## 📁 Project Structure

The repository is organized as follows:

- `main.tf`: Main file that defines the resources to be provisioned.
- `providers.tf`: Configures the providers used, such as AWS.
- `variables.tf`: Declares the variables used in the project.
- `outputs.tf`: Defines the outputs that will be shown after applying Terraform.
- `modules/`: Directory for reusable modules, promoting modularization and code reuse.

## ✅ Prerequisites

Before starting, make sure you have installed:

- [Terraform](https://developer.hashicorp.com/terraform/downloads)
- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
- An [AWS account](https://aws.amazon.com/)

Also, configure your AWS credentials:

```bash
aws configure
```

## 🚀 How to Use

1. **Clone the repository:**

   ```bash
   git clone https://github.com/FelipeFardo/Terraform-First-Iac.git
   cd Terraform-First-Iac
   ```

2. **Initialize Terraform:**

   ```bash
   terraform init
   ```

3. **Preview the execution plan:**

   ```bash
   terraform plan
   ```

4. **Apply the configuration:**

   ```bash
   terraform apply
   ```

   Confirm the execution by typing `yes` when prompted.

5. **(Optional) Destroy the provisioned infrastructure:**

   ```bash
   terraform destroy
   ```

## 📌 Notes

- Ensure your AWS credentials have sufficient permissions to create and manage the defined resources.
- You can adjust the variable values in the `variables.tf` file as needed.
- Use the modules within the `modules/` directory to organize and reuse common configurations.

## 📄 License

This project is licensed under the [MIT License](LICENSE).
