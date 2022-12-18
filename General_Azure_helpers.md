- Paired-regions: https://learn.microsoft.com/en-in/azure/reliability/cross-region-replication-azure#azure-cross-region-replication-pairings-for-all-geographies
- Architect Azure applications for resiliency and availability: https://learn.microsoft.com/en-in/azure/architecture/reliability/architect
- Active geo-replication: https://learn.microsoft.com/en-in/azure/azure-sql/database/active-geo-replication-overview?view=azuresql
- Azure Storage redundancy: https://learn.microsoft.com/en-in/azure/storage/common/storage-redundancy
- Highly available multi-region web application: https://learn.microsoft.com/en-in/azure/architecture/reference-architectures/app-service-web-app/multi-region
- Continuous deployment to Azure App Service: https://learn.microsoft.com/en-in/azure/app-service/deploy-continuous-deployment?tabs=github
- Traffic routing methods to origin: https://learn.microsoft.com/en-in/azure/frontdoor/routing-methods#priority-based-traffic-routing
- Decision tree for load balancing in Azure: https://learn.microsoft.com/en-in/azure/architecture/guide/technology-choices/load-balancing-overview#decision-tree-for-load-balancing-in-azure


Front Door: Front Door routes incoming requests to the primary region. If the application running in that region becomes unavailable, Front Door fails over to the secondary region.

A multi-region deployment can use an active-active or active-passive configuration. An active-active configuration distributes requests across multiple active regions. An active-passive configuration keeps warm instances in the secondary region, but doesn’t send traffic there unless the primary region fails.
