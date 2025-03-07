---
title: What's new?
description: Learn about the new features for and improvements to SQL Server on Azure Virtual Machines.
author: MashaMSFT
ms.author: mathoma
ms.reviewer: randolphwest, mathoma
ms.date: 03/01/2024
ms.service: virtual-machines-sql
ms.subservice: service-overview
ms.topic: whats-new
ms.custom: ignite-2023
tags: azure-service-management
---
# What's new with SQL Server on Azure Virtual Machines?

[!INCLUDE[appliesto-sqlvm](../../includes/appliesto-sqlvm.md)]

> [!div class="op_single_selector"]
> * [Azure SQL Database](../../database/doc-changes-updates-release-notes-whats-new.md?view=azuresql&preserve-view=true)
> * [Azure SQL Managed Instance](../../managed-instance/doc-changes-updates-release-notes-whats-new.md?view=azuresql&preserve-view=true)
> * [SQL Server on Azure VMs](doc-changes-updates-release-notes-whats-new.md?view=azuresql&preserve-view=true)

When you deploy an Azure virtual machine (VM) with SQL Server installed on it, either manually, or through a built-in image, you can use Azure features to improve your experience. This article summarizes the documentation changes associated with new features and improvements in the recent releases of [SQL Server on Azure Virtual Machines (VMs)](https://azure.microsoft.com/services/virtual-machines/sql-server/). To learn more about SQL Server on Azure VMs, see the [overview](sql-server-on-azure-vm-iaas-what-is-overview.md). 

For updates made in previous years, see the [What's new archive](doc-changes-updates-release-notes-whats-new-archive.md). 

[!INCLUDE [entra-id](../../includes/entra-id.md)]


## Preview

The following table lists the features of SQL Server on Azure VMs that are currently in preview.

> [!NOTE]  
> Features currently in preview are available under [supplemental terms of use](https://azure.microsoft.com/support/legal/preview-supplemental-terms/), review for legal terms that apply to Azure features that are in beta, preview, or otherwise not yet released into general availability. SQL Server on Azure VMs provide previews to give you a chance to evaluate and [share feedback with the product group](https://feedback.azure.com/d365community/forum/04fe6ee0-3b25-ec11-b6e6-000d3a4f0da0) on features before they become generally available (GA).

| Feature | Details |
| --- | --- |
| [Azure SQL triggers for Azure Functions](/azure/azure-functions/functions-bindings-azure-sql-trigger) | Azure Functions supports function triggers for Azure SQL Database. |
| [Azure Update Manager](../azure-update-manager-sql-vm.md) | Automatically patch multiple SQL Server VMs at scale with the Azure Update Manager integrated in to the [SQL virtual machines](manage-sql-vm-portal.md) resource in the Azure portal, including Cumulative Updates. |
| [Premium SSD v2 in the Azure portal](storage-configuration-premium-ssd-v2.md) | Provision your SQL Server on Azure VM with Premium SSD v2 disks in the Azure portal for improved throughput and performance. |  

## General availability (GA)

The following table lists features of SQL Server on Azure VMs that have been made generally available (GA) within the last 12 months:

| Changes | Month | Details |
| --- | --- |--- |
| [Azure Elastic SAN](performance-guidelines-best-practices-storage.md#azure-elastic-san) | February 2024 | Place your SQL Server workloads on an Azure Elastic SAN for improved performance, throughput, and cost. | 
| [SQL VM health notifications](manage-sql-vm-portal.md#overview-page) | September 2023 | The **Overview** page of the SQL virtual machines resource in the Azure portal now displays information about the health of the [SQL IaaS Agent extension](sql-server-iaas-agent-extension-automate-management.md), as well as error conditions when the state is _unhealthy_ or _failed_. Review [Troubleshoot the extension](sql-agent-extension-troubleshoot-known-issues.md) to learn more. | 
| [Configure AG from Azure portal](availability-group-azure-portal-configure.md) | August 2023 | Deploy an Always On availability group to multiple subnets by using the Azure portal. |
| [Azure SQL bindings for Azure Functions](/azure/azure-functions/functions-bindings-azure-sql) | May 2023 | Azure Functions supports input bindings, and output bindings for the Azure SQL and SQL Server products. | 
| [Auto upgrade SQL IaaS Agent extension](manage-sql-vm-portal.md#sql-iaas-agent-extension-settings) | April 2023 | It's now possible to enable the automatic upgrade of your SQL IaaS Agent extension to ensure you're automatically receiving the latest updates to the extension every month |
| [Microsoft Entra authentication](configure-azure-ad-authentication-for-sql-vm.md) | April 2023 | Configure Microsoft Entra authentication for your SQL Server on Azure VMs. |  

## Documentation changes 

Learn about significant changes to the SQL Server on Azure VMs documentation. For previous years, see the [What's new archive](doc-changes-updates-release-notes-whats-new-archive.md).

### March 2024

| Changes | Details |
| --- | --- |
| **Deploy SQL VM with Premium SSD v2 in Azure portal preview** | For improved throughput and performance, provision your SQL Server on Azure VMs with Premium SSD v2 disks by using the Azure portal.  Deploying your SQL Server VMs with Premium SSD v2 in the Azure portal is currently in preview. To learn more, review [Deploy SQL Server on Azure VMs with Premium SSD v2](storage-configuration-premium-ssd-v2.md). | 


## February 2024

| Changes | Details |
| --- | --- |
|**Azure Elastic SAN GA** | You can now place your SQL Server workloads on an Azure Elastic SAN for improved performance, throughput, and cost. The Azure Elastic SAN is now generally available (GA).  Review [Azure Elastic SAN](performance-guidelines-best-practices-storage.md#azure-elastic-san) to learn more.| 
|**Configure log shipping** | Learn to configure log shipping between two SQL Server on Azure VMs. Review [Configure log shipping](log-shipping-configure.md) to learn more. |


## October 2023

| Changes | Details |
| --- | --- |
| **Azure Elastic SAN preview** | You can now place your SQL Server workloads on an Azure Elastic SAN for improved performance, throughput, and cost. The Azure Elastic SAN is currently in preview. Review [Azure Elastic SAN](performance-guidelines-best-practices-storage.md#azure-elastic-san) to learn more. |  

## September 2023

| Changes | Details |
| --- | --- |
| **SQL VM health notifications** |  The **Overview** page of the [SQL virtual machines](manage-sql-vm-portal.md#overview-page) resource in the Azure portal now displays information about the health of the [SQL IaaS Agent extension](sql-server-iaas-agent-extension-automate-management.md), as well as error conditions when the state is _unhealthy_ or _failed_. Review [Troubleshoot the extension](sql-agent-extension-troubleshoot-known-issues.md) to learn more. | 
| **Microsoft Entra ID rebrand**|  Azure Active Directory has been rebranded to [Microsoft Entra ID](/entra/fundamentals/new-name). | 


## Archive

For updates made in previous years, see the [What's new archive](doc-changes-updates-release-notes-whats-new-archive.md). 

## Contribute to content

To contribute to the Azure SQL documentation, see the [Docs contributor guide](/contribute/).

## Additional resources

**Windows VMs**:

* [Overview of SQL Server on Windows VMs](sql-server-on-azure-vm-iaas-what-is-overview.md)
* [Provision SQL Server on Windows VMs](create-sql-vm-portal.md)
* [Migration guide: SQL Server to SQL Server on Azure Virtual Machines](../../migration-guides/virtual-machines/sql-server-to-sql-on-azure-vm-individual-databases-guide.md)
* [High availability and disaster recovery for SQL Server on Azure Virtual Machines](business-continuity-high-availability-disaster-recovery-hadr-overview.md)
* [Performance best practices for SQL Server on Azure Virtual Machines](./performance-guidelines-best-practices-checklist.md)
* [Application patterns and development strategies for SQL Server on Azure Virtual Machines](application-patterns-development-strategies.md)

**Linux VMs**:

* [Overview of SQL Server on a Linux VM](../linux/sql-server-on-linux-vm-what-is-iaas-overview.md)
* [Provision SQL Server on a Linux virtual machine](../linux/sql-vm-create-portal-quickstart.md)
* [FAQ (Linux)](../linux/frequently-asked-questions-faq.yml)
* [SQL Server on Linux documentation](/sql/linux/sql-server-linux-overview)
