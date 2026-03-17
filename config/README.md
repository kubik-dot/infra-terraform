import os
import subprocess

def main():
    # Get the current directory
    current_dir = os.getcwd()

    # Change into the Terraform directory
    terraform_dir = os.path.join(current_dir, 'terraform')
    os.chdir(terraform_dir)

    # Initialize Terraform
    subprocess.run(['terraform', 'init'])

    # Format the Terraform code
    subprocess.run(['terraform', 'fmt'])

    # Validate the Terraform code
    subprocess.run(['terraform', 'validate'])

    # Apply the Terraform configuration
    subprocess.run(['terraform', 'apply', '-auto-approve'])

if __name__ == '__main__':
    main()