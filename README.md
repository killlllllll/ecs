# Infrastructure Provisioning for Projects via Terraform

Mono repo for all projects IaC and its automated deployment

# Folder Structure

```
modules |  -> All Terraform modules
|       |
|       services  | -> TF Modules for each type of service (eg: strapi, react-frontend, express-backend)
|       |         |
|       |        <service A (type of frontend/backend)>
|       |        <service B (type of frontend/backend)> 
|       resources |
|                 |
|                 <resource name (aws-s3, aws-ecs, aws-cloudfront)>
|               
<project-name> |
               |
                <env (dev/stage/prod)> 
                         |
                         |
                         main.tf
                         variables.tf
                         providers.tf
```

