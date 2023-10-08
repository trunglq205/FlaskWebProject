# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
    I. Virtual Machine (VM):
        1. Costs:
            a. VMs can be cost-effective for long-term or predictable workloads. You pay for the VM's uptime.
            b. Costs include VM provisioning, storage, and possibly additional services like load balancers.

        2. Scalability:
            a. VMs offer flexibility in terms of scalability, but it requires manual intervention to resize or add more VM instances.
            b. You can set up auto-scaling, but it adds complexity and cost.

        3. Availability:
            a. VMs can achieve high availability through load balancing, replication, and failover configurations.
            b. Achieving high availability often requires more effort and additional cost.

        4. Workflow:
            a. VMs provide more control over the entire infrastructure, making it suitable for complex app setups.
            b. You need to manage the OS updates, security patches, and software installations.

    II. Azure App Service:
        1. Costs:
            a. App Service is a platform-as-a-service (PaaS) offering with a more predictable and potentially lower cost structure.
            b. You pay for the compute resources your app consumes, and Azure handles much of the underlying infrastructure.

        2. Scalability:
            a. App Service offers easy scalability with auto-scaling options based on CPU or memory usage.
            b. Scaling is automated and can handle traffic spikes efficiently.

        3. Availability:
            a. Azure App Service provides built-in high availability and load balancing.
            b. It includes features like deployment slots for seamless updates and rollback.

        4. Workflow:
        a. App Service simplifies the deployment process with easy integration into CI/CD pipelines.
        b. It abstracts much of the infrastructure management, allowing developers to focus on code.

- *Choose the appropriate solution (VM or App Service) for deploying the app*
    => For a CMS app, I recommend using Azure App Service

- *Justify your choice*
    => While VMs offer more control and are suitable for certain scenarios, the simplicity, cost-effectiveness, and ease of management provided by Azure App Service make it a strong choice for hosting a CMS app, particularly if your primary focus is on the application itself rather than the infrastructure.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 