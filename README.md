# Cloud Resume Challenge - Frontend Serverless GCP
### Serverless resume on GCP with API backend and GitOps-based CI/CD

This repository hosts the frontend code and setup instructions for implementing the Cloud Resume Challenge using Google Cloud Platform (GCP).

### Challenge Overview

The Cloud Resume Challenge is a hands-on project to build a personal resume website and host it entirely on GCP infrastructure. Build a secure and scalable personal resume website using GCP and modern tooling. Showcase cloud skills, web development understanding with Hugo, containerization practices, Cloud Run deployment, and IaC proficiency with Terraform.


### Project Requirements

1. **Terraform Configuration:** Write Terraform configuration files (`.tf`) to provision the following:
   - Custom VPC Network
   - Cloud Load Balancer (Internal) with HTTPS configuration
   - Cloud CDN integration
   - Cloud DNS records for your custom domain

2. **Hugo for Templating:** Use Hugo to generate your HTML resume and manage CSS styling. 

3. **Distroless Cloud Build:**  Employ Cloud Build to create streamlined, distroless container images of your Hugo website.

4. **Cloud Run Deployment:** Deploy the containerized website on Cloud Run.

5. **Custom Domain:** Employ Cloud Domains (or your preferred provider) to register a custom domain name.

#### Technologies Used**

* Terraform
* Hugo
* HTML 
* CSS
* Google Cloud Build
* Google Cloud Run
* Google Cloud Load Balancing
* Google Cloud CDN
* Google Cloud Domains (or an alternative DNS provider)
* Google Cloud VPC

### Getting Started

1. **Prerequisites:**
   - A Google Cloud Platform account.
   - Basic understanding of Hugo, web hosting, VPC networking, containerization, and Terraform.
   - Hugo installed locally.
   - Terraform installed locally.

2. **Write Terraform configuration files to define your GCP infrastructure.** 

3. **Set up a Hugo project with your resume content and styling.**

4. **Write a Cloud Build configuration file (`cloudbuild.yaml`) to:**
   - Build your Hugo site
   - Create a distroless container image 

5. **Deploy:**
   - Use `terraform init` and `terraform apply` to deploy your infrastructure.
   - Use `gcloud run deploy` to deploy the container image to Cloud Run, referencing resources provisioned by Terraform.