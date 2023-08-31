# JENKINS-CI-CD-PIPELINE-TO-BUILD-AND-DEPLOY-DOCKER-CONTAINER-TO-KUBERNETES-CLUSTER


Problem Statement:


![image](https://github.com/manasthorat/JENKINS-CI-CD-PIPELINE-TO-BUILD-AND-DEPLOY-DOCKER-CONTAINER-TO-KUBERNETES-CLUSTER/assets/55976364/b03bf762-41c3-4180-9ba7-a642b53128a5)

Solution:

Git Workflow and Version Control: Established an efficient Git workflow that facilitated version control, feature branching, and pull requests. Implemented monthly releases on the 25th, ensuring organized and controlled deployments.

CodeBuild Integration: Configured a Git webhook to trigger CodeBuild on each commit to the master branch. This automation reduced manual intervention and streamlined the build process.

Containerization with Docker: Designed a Dockerfile to containerize the application. Set up automated Docker image builds triggered by GitHub pushes, ensuring consistent and reproducible deployments.

Kubernetes Deployment and Scaling: Orchestrated the deployment of containerized application using Kubernetes on AWS. Implemented 2 replicas for high availability and created a NodePort service on port 30008 for external access.

Jenkins Pipeline Automation: Developed a Jenkins Pipeline script to automate the entire process, from code checkout to Kubernetes deployment. Integrated secure Docker Hub image pushes and Kubernetes configurations.

Infrastructure Creation with Terraform: Utilized Terraform to provision AWS infrastructure. Set up Worker instances with specific software installations based on their designated roles, promoting consistent configuration.

Configuration Management with Ansible: Employed Ansible playbooks to configure software on designated worker machines. Ensured the proper installation of Java, Docker, Kubernetes, Jenkins, and other dependencies.


Project Architecture:


The project architecture comprised several components working in harmony:

GitHub Repository: Hosted the application source code and Dockerfile, enabling version control and collaboration.

Git Workflow: Implemented a structured Git workflow that facilitated feature development, pull requests, and monthly releases on the 25th.

CodeBuild: Automated build process triggered by Git commits, ensuring that the latest code changes were built into Docker images.

Docker Hub: Container images were pushed to Docker Hub, providing a central repository for sharing and distribution.

Kubernetes Cluster: Utilized AWS resources to set up a Kubernetes cluster responsible for orchestrating application deployment and scaling.

Jenkins Pipeline: A scripted pipeline orchestrated the end-to-end process, from code checkout to Kubernetes deployment. Secured Docker Hub credentials were managed within the pipeline.

Terraform Infrastructure: Employed Terraform to create and manage AWS infrastructure, including Worker instances with specific roles.

Ansible Configuration Management: Ansible playbooks ensured consistent software installation across Worker machines based on their designated roles.

Outcome: The project resulted in an automated DevOps lifecycle that enabled Analytics Pvt Ltd to seamlessly deploy, scale, and operate the containerized product. The modern architecture enhanced development efficiency, reduced manual interventions, and ensured reliable and consistent deployments, ultimately contributing to the product's success and customer satisfaction.






