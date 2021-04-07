---
title: "MetaOmics Server"
output:
  html_document:
    toc: yes
pagetitle: MetaOmics Server
---
# MetaOmics Server

This server is intended to support analysis and visualisation of omics research. 
In particular the visualisation of multiple omics datasets, thereby enabling better integration, comparison and utilisation. 

## Hardware

<details><summary></summary>
<p>

Dell PowerEdge

- 2x 40 Cores (80 Threads)
- 256GB of RAM
- 5x 8TB HDD as RAID 5 = 25TB
- 2x 3.48TB SSD = 6.94TB as scratch disk.
 
[Full specifications](https://teams.microsoft.com/l/file/EA5BDA05-3E27-49FC-B5B4-09E18A9EDD59?tenantId=92454335-564e-4ccf-b0b0-24445b8c03f7&fileType=pdf&objectUrl=https%3A%2F%2Fuctcloud.sharepoint.com%2Fsites%2FMetaOmics%2FShared%20Documents%2FGeneral%2FDell_PowerEdge%2FQUOTEPLUS_ZA_REL_ENTP_13005405.2_2020_04_28.pdf&baseUrl=https%3A%2F%2Fuctcloud.sharepoint.com%2Fsites%2FMetaOmics&serviceName=teams&threadId=19:69aefdfd8fae438b8711b71b1be109a2@thread.tacv2&groupId=1ca5c006-1beb-4523-9772-ce69d774b54d)

[Technical Guide](https://teams.microsoft.com/l/file/7D4D75FA-9593-4C8A-9E41-EE04BFA78A64?tenantId=92454335-564e-4ccf-b0b0-24445b8c03f7&fileType=pdf&objectUrl=https%3A%2F%2Fuctcloud.sharepoint.com%2Fsites%2FMetaOmics%2FShared%20Documents%2FGeneral%2FDell_PowerEdge%2FPowerEdge_R740_R740xd_Technical_Guide.pdf&baseUrl=https%3A%2F%2Fuctcloud.sharepoint.com%2Fsites%2FMetaOmics&serviceName=teams&threadId=19:69aefdfd8fae438b8711b71b1be109a2@thread.tacv2&groupId=1ca5c006-1beb-4523-9772-ce69d774b54d)



## Access

Admin for this server is [Shaun Garnett](shaun.garnett@uct.ac.za) from the Blackburn Lab and [Heine De Jager](Heine.dejager@uct.ac.za) from ICTS. Correspondence should be first with Shaun. 



Users gain access through their UCT credentials and passwords

[List of Users](https://teams.microsoft.com/l/file/C027AC14-D705-48C9-BCE9-E799EF1DA1E6?tenantId=92454335-564e-4ccf-b0b0-24445b8c03f7&fileType=xlsx&objectUrl=https%3A%2F%2Fuctcloud.sharepoint.com%2Fsites%2FMetaOmics%2FShared%20Documents%2FGeneral%2FServer_Access.xlsx&baseUrl=https%3A%2F%2Fuctcloud.sharepoint.com%2Fsites%2FMetaOmics&serviceName=teams&threadId=19:69aefdfd8fae438b8711b71b1be109a2@thread.tacv2&groupId=1ca5c006-1beb-4523-9772-ce69d774b54d)


## Virtual Machines

The server is running a Hyper-V server. This will host a number of virtual server. Some will be always on allowing access to shiny-server apps, while others will be On-Demand. 

### Always on

Servers that are always accessible

<details><summary></summary>
<p>

#### [MetaOmics Shiny-Server](https://teams.microsoft.com/l/channel/19%3A8f8f3c4354164a3480d54d9e3ec0c9e5%40thread.tacv2/tab%3A%3A24801d3a-52c1-44e8-8b73-f2b9dc1b24b8?groupId=1ca5c006-1beb-4523-9772-ce69d774b54d&tenantId=92454335-564e-4ccf-b0b0-24445b8c03f7)

<details><summary></summary>
<p>

This server will host a shiny-server app for analysis and visualising omics data

- Ubuntu : Shiny Server : 64 Threads 198 GB of RAM
- Always on
- Access to shiny-server from off campus, via Firewall rule
- IP Address : 137.158.163.205





#### MySQL server

<details><summary></summary>
<p>

Request Access from [Shaun Garnett](shaun.garnett@uct.ac.za)

Host : srvubusql007.uct.ac.za

```mysql -h srvubusql007.uct.ac.za -u username -p```



 
### On Demand



Variable sized configuration depending on demand of analysis. Able to access all free resources
Individual images, that can be launched on demand

<details><summary></summary>
<p>

#### Linux Server

<details><summary></summary>
<p>

Ubuntu server 

Base Configuration

- 24 Cores and 64 GB of RAM

#### Windows Server

##### Windows Virtual Machines

Windows Virtual machines that can be launched on demand. Different sized machines will be available for different sized jobs

[Link to Configuration Information](https://teams.microsoft.com/l/channel/19%3A29ca9462fa264c428bc13b9448ca8ddc%40thread.tacv2/tab%3A%3A0e09d175-de68-4aef-8564-1f2e005fb9a1?groupId=1ca5c006-1beb-4523-9772-ce69d774b54d&tenantId=92454335-564e-4ccf-b0b0-24445b8c03f7)








## Storage Space

Should be mounted on all virtual server

### Local

#### SSD

2x 3.48TB SSD = 6.94TB

#### HDD

5x 8TB HDD as RAID 5 = 25TB

### Research Data

#### BlackburnLab

 - 25 TB of backed up storage space for Blackburn Lab
 - mounted at ``` /mnt/ResearchData/```

#### BlackburnArchive

 - 25TB
 - mounted at ``` /mnt/Archive ```

### NAS

#### crick

9TB RAID5