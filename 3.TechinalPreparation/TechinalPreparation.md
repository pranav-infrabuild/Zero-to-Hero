<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=28&color=00F72B&center=true&vCenter=true&width=800&lines=DevOps+Interview+Preparation;Zero+to+Hero+🚀;Crack+Your+Next+Job" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Level-Beginner_to_Advanced-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" />
</p>

---

## 💻 Technical Interview Questions

---

### 1. Which tools and technologies have you worked on❓
<details>
<summary>👉 Click to view answer</summary>

I have worked on **Git, Linux, Docker, Kubernetes, Terraform, Prometheus, and Grafana**.  
Apart from this, I have also used **ServiceNow, Jira, and Azure services**.

</details>

---

### 2. Which Azure services do you know most❓
<details>
<summary>👉 Click to view answer</summary>

I mainly work with **Azure DevOps, Virtual Machines, Storage Accounts, Azure Kubernetes Service (AKS)**, and networking services like **VNet and Load Balancer**.  
I have also worked with **Azure Monitor and Azure Key Vault**.

</details>

---

### 3. Have you worked on Azure Functions or Logic Apps❓
<details>
<summary>👉 Click to view answer</summary>

I have basic knowledge of **Azure Functions and Logic Apps**, but my main hands-on experience is with core services like **Azure DevOps, AKS, and Virtual Machines**.

</details>

---

### 4. Which Linux OS have you worked on❓
<details>
<summary>👉 Click to view answer</summary>

I have worked mainly on **Ubuntu**.  
The current latest version is **Ubuntu 24.04 LTS**.

To install and manage packages, I use **APT (Advanced Package Tool)**.

</details>

---

### 5. Tell me about yourself / Introduction ❓
<details>
<summary>👉 Click to view answer</summary>

Hi, my name is XYZ. I completed my Bachelor’s degree in Mechanical Engineering from **Savitribai Phule Pune University** with First Class Distinction.

Currently, I am based in Hinjewadi, Pune. I joined [Company Name] in 2021, and since then I have been working as a DevOps Engineer.

During this time, I have worked on major projects, including a core Azure DevOps project where I gained hands-on experience with tools and technologies such as Git, Linux, Docker, Kubernetes, Helm, Prometheus, and Grafana.

Talking about my achievements, I have completed certifications like [Certification Names].

At present, I am continuously upskilling myself and looking forward to contributing my best to the organization and delivering value to clients.

Thank you.

</details>

---

### 6. What is Continuous Integration, Continuous Delivery, Continuous Deployment ❓
<details>
<summary>👉 Click to view answer</summary>

### 1. **Continuous Integration (CI):**   
   - **What it is:** Continuous Integration is a practice where developers frequently integrate their code changes into a shared repository, usually several times a day.
   - **Why it’s important:** Every time code is integrated, it is automatically tested. This helps catch bugs early and ensures that the new code works well with the existing code.
   
### 2. **Continuous Delivery (CD):**
   - **What it is:** Continuous Delivery is an extension of Continuous Integration. After the code is integrated and tested, it is automatically prepared for deployment to production (or a live environment), but the deployment itself might still require manual approval.
   
### 3. **Continuous Deployment (CD):**
   - **What it is:** Continuous Deployment takes Continuous Delivery a step further by automatically deploying every change that passes the tests directly to production, without any manual approval.

</details>

---

### 7. What is azure Devops❓
<details>
<summary>👉 Click to view answer</summary>

Azure DevOps is a popular choice for several reasons, especially if you’re involved in software development and operations. Here’s why Azure DevOps might be the right tool for you:

### 1. **All-in-One Platform:**
   - **What it is:** Azure DevOps offers a comprehensive suite of tools for every stage of the software development lifecycle (SDLC) – from planning and coding to testing, releasing, and monitoring.
   - **Why it’s important:** You don’t need to switch between different tools for different tasks. Everything you need is integrated into one platform, which simplifies the workflow.

</details>

---

### 8. Explain your Project CI/CD Pipeline❓
<details>
<summary>👉 Click to view answer</summary>

I am working for multiple development team as a DevOps Engineer 
Mostly the projects are Based on Java application 

In that project I use GitHub as a version control system and target was the kubernates cluster 

Whenever any developer commit the code , we will check out the commit code. With the git hub webhooks that repo automatically push to azure DevOps.
And start the performing build action 
We use maven for building.

After that we will scan the code  for any vulnerability with the help of Sonarcloud. 
Also perform security checks. In this stage, the code is scanned for vulnerabilities using Sonarcloud 

Once the code passes all tests and scans, a Docker  image  building process will be started . After building the image, it’s scanned for vulnerabilities through trivy. In this stage checking the base image and other dependencies for security issues happened.

Once the image passes all checks, it’s pushed to an image registry like Docker Hub registry with latest tag

After the image is pushed, the next step is to deploy this image to the Kubernetes platform. Now deployed using Helm Charts, These charts include configurations for pulling the Docker image from the registry, setting up Kubernetes resources, and managing environment-specific configurations.

After that we deploy application through the Helm Chart to your Kubernetes Cluster.


</details>

---

### 9. What is u r day to day Activities❓
<details>
<summary>👉 Click to view answer</summary>

Coming to the my day to day activities our organization uses a service now tool as a task management.
We are working on multiple projects so on daily basis usually gets an 10-11 tickets based on Developers and user requirements.
We are following agile methodologies so product owner decide the priority of that task.

Usually Task list like

1) Getting Cpu Utilization Error or Server Slow Response 

<details>
**Interviewer:** Can you describe a scenario where you need to troubleshoot a performance issue on a Linux server?

**Answer:** Certainly. Let's assume there's a web application running on a Linux server, and users are reporting slow response times. The first step would be to check the system resource utilization using commands like `top`, `htop`, or `ps`. These tools provide an overview of CPU, memory, and disk usage, helping identify potential bottlenecks.

**Interviewer:** Let's say the CPU usage is high. How would you identify the processes consuming the most CPU?

**Answer:** If the CPU usage is high, I would start by using the `top` command, which allows me to sort processes by CPU usage in real-time. Another option is to use `ps` with flags like `aux --sort=-%cpu`, which lists processes sorted by CPU consumption. Once I identify the resource-intensive processes, I would dig deeper to understand why they're using so much CPU, checking for things like runaway processes, misconfigurations, or inefficient code.

**Interviewer:** Suppose the CPU usage seems normal, but the memory usage is high. How would you troubleshoot this issue?

**Answer:** If memory usage is the concern, I would use commands like `free -m` or `vmstat` to get a snapshot of memory utilization. To pinpoint which process is consuming the most memory, I could use `ps` with options like `aux --sort=-%mem`. In cases of high memory usage, I'd investigate for memory leaks in the application code, excessive caching, or misconfigured memory settings. Depending on the findings, I might tweak the application's memory limits, optimize the code, or consider adding more RAM to the server.

**Interviewer:** What steps would you take if you suspect disk I/O is causing the performance issue?

**Answer:** To diagnose disk I/O issues, I would use tools like `iostat` or `iotop` to monitor disk activity and identify any processes responsible for high I/O operations. I would also check for disk bottlenecks such as a nearly full disk, filesystem fragmentation, or failing drives. If disk I/O is indeed the issue, I might optimize the filesystem, upgrade to faster storage (like SSDs), or distribute the load across multiple disks to improve performance.

</details>


2) Geting tickets from user saying they unable to ran script or job
<details>

To add a user to a specific group in a Linux environment, you can follow these steps. Assuming you have SSH access to the server and the necessary privileges, here's how you can add a user to a group:

### 1. **Check if the User Exists**
   Before adding a user to a group, you should check if the user exists. You can do this by running:
   ```bash
   id username
   ```
   Replace `username` with the actual username. If the user exists, you will see their user ID (UID), group ID (GID), and the groups they are a part of.

### 2. **Check if the Group Exists**
   Verify if the group (in this case, the Python group) exists by running:
   ```bash
   getent group groupname
   ```
   Replace `groupname` with the actual group name. This will list the group and its members if it exists.

### 3. **Add the User to the Group**
   To add a user to the group, use the following command:
   ```bash
   sudo usermod -aG groupname username
   ```
   Replace `groupname` with the name of the group (e.g., `python`) and `username` with the user's name. The `-aG` option adds the user to the group without affecting their membership in other groups.

### 4. **Verify the User’s Group Membership**
   After adding the user, you can verify their membership by running:
   ```bash
   groups username
   ```
   This command will list all the groups that the user is a member of, including the newly added one.

### 5. **Inform the User**
   Once you’ve added the user to the group, inform them that they now have access to run the necessary jobs. You can update them via email, a ticketing system, or your internal communication platform.

### Example:
   Suppose you have a user named `johndoe` and you want to add them to a group called `python`, you would run:
   ```bash
   sudo usermod -aG python johndoe
   ```
   Then check the groups:
   ```bash
   groups johndoe
   ```

This will ensure that `johndoe` is added to the `python` group and can run the jobs as needed.

</details>

3) set up an promothes and graphana for application 
<details>

https://www.coachdevops.com/2022/05/how-to-setup-monitoring-on-kubernetes.html?m=1
</details>

4) creat an 10 users with xyz iam roles
<details>
 
**Daily Task Explanation: Creating Users with IAM Roles for AKS Clusters**

As an Azure DevOps Engineer, one of my daily tasks involves creating and managing user accounts with specific IAM roles for Azure Kubernetes Service (AKS) clusters 

### 1. **Creating Users and Assigning IAM Roles for AKS Clusters**

1. **Identify User Requirements:**
   - Determine the role and responsibilities for each user based on their function within the AKS environment. For example, some users might need read-only access, while others might need full admin rights.

2. **Azure Portal:**

   - **Azure Portal:**
     - Navigate to the Azure Portal.
     - Go to the AKS cluster resource.
     - Under “Access control (IAM),” click on “Add role assignment.”
     - Assign appropriate roles (e.g., Kubernetes Cluster Admin, Kubernetes Cluster User) to each user.


</details>

4) modify the pipeline by more secure way :- trivy for docker image
<details>

To enhance the security of your CI/CD pipeline, integrating Trivy for scanning Docker images is a good practice. Trivy is a comprehensive security scanner that detects vulnerabilities in open-source packages, OS packages, and Docker images. Here's a step-by-step guide on how to modify your pipeline to include Trivy for Docker image scanning:

### 1. **Install Trivy in the Pipeline**
   - Ensure that Trivy is available in the pipeline environment. You can install Trivy as part of your CI job by adding the following command:
   
   ```bash
   curl -sfL https://raw.githubusercontent.com/aquasecurity/trivy/main/contrib/install.sh | sh
   ```

### 2. **Scan Docker Image**
   - Add a step in your pipeline to scan the Docker image using Trivy. Here's an example of how you can do this:

   ```yaml
   stages:
     - build
     - test
     - scan
     - deploy

   scan:
     stage: scan
     script:
       - trivy image --exit-code 1 --severity HIGH,CRITICAL my-app:latest
     allow_failure: false
   ```

   In this example:
   - The `--exit-code 1` flag will cause the job to fail if vulnerabilities with the specified severities (HIGH, CRITICAL) are found.
   - The `--severity HIGH,CRITICAL` flag ensures that only vulnerabilities of high and critical severity levels are flagged.

### 3. **Store and Review Scan Reports**
   - Optionally, store the scan reports for auditing purposes and review them to ensure no vulnerabilities are introduced into your Docker images. You can redirect the scan output to a file:

   ```yaml
   scan:
     stage: scan
     script:
       - trivy image --exit-code 1 --severity HIGH,CRITICAL --format json --output trivy-report.json my-app:latest
     allow_failure: false
     artifacts:
       paths:
         - trivy-report.json
   ```

### 4. **Automate Security Checks**
   - Integrate the Trivy scan with your CI/CD pipeline to automatically block deployments if vulnerabilities are detected. This can be crucial for preventing insecure images from reaching production.

### 5. **Configure Alerts and Notifications**
   - Set up alerts or notifications to inform the relevant teams when vulnerabilities are found, allowing for quick remediation.


</details>

6) Some of the application not working on aks kubernates pod 
<details>
</details>   

7) pod management
<details>
1. crashloopbackoffstate
2. imagepullbackoff
3. Pod is in Pending State  
</details>
   
8) monitoring the pods through tools 


</details>

---

### 10:- How is your branching strategy in your Azure Repo❓
<details>
<summary>👉 Click to view answer</summary>

My team follows a structured branching strategy in our Azure Repos to ensure smooth collaboration and code stability across different stages of the development cycle.

1. **Main Branch (Production)**:  
   This is our most critical branch. It's always kept stable production-ready code. Only thoroughly tested and reviewed code gets merged into this branch, usually via pull requests.

2. **Develop Branch**:  
   We have a 'develop' branch, which is the default branch for all new features. Developers create feature branches from 'develop,' work on new functionality, and then merge back to 'develop' after code reviews and testing. This ensures that the 'develop' branch is always up-to-date with the latest changes. This branch represents the upcoming version of the application

3. **Feature Branches**:  
   For any new development or task, we create a separate feature branch named after the task (e.g., `feature/add-user-authentication`). This keeps our work isolated and ensures that incomplete features don't affect the main codebase. Once a feature is completed, it goes through a code review process before merging back into the 'develop' branch.

4. **Release Branches**:  
   When we are preparing for a release, we create a release branch (e.g., `release/v1.2`). This allows us to freeze features and focus on final testing and bug fixing. Only critical fixes are merged into the release branch. Once it's stable, we merge the release branch into both the 'main' and 'develop' branches.

5. **Hotfix Branches**:  
   In case of any urgent issues in production, we create hotfix branches from the 'main' branch (e.g., `hotfix/issue-123`). These branches allow us to address critical problems quickly. Once fixed, the hotfix branch is merged into both the 'main' and 'develop' branches to ensure that the fix is included in future releases.
   

</details>

---
