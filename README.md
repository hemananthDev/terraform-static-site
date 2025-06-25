# Static Website Hosting with Terraform

This project provisions a static website on AWS using:

- **S3** for hosting HTML files
- **IAM** for access policy
- **CloudFront** as CDN
- **Terraform** for IaC

## Project Structure

- `/my-static-site/` – HTML content
- `/terraform-static-site/` – Terraform code

## Usage

1. `cd terraform-static-site`
2. `terraform init`
3. `terraform apply`
4. Upload HTML files to S3:
   ```bash
   aws s3 cp ../my-static-site/ s3://<your-bucket> --recursive
