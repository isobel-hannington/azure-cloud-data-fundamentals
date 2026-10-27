# ☁️ Azure: cloud and data fundamentals (DP-900)

**Cloud concepts, a costed estimate and a client recommendation, plus Microsoft's DP-900 guided labs on data in Azure and Microsoft Fabric.**

From Week 5 of my bootcamp. I researched how cloud computing works, priced an enterprise BI solution and advised a client on moving its database servers to the cloud. I then worked through Microsoft's DP-900 guided labs on relational, non-relational and analytical data, and covered the UK law on computer use and data.

## 🔎 At a glance

| | |
|---|---|
| **Tools** | Azure Pricing Calculator. In the guided labs: Azure SQL Database, Azure Storage, Azure Cosmos DB, Microsoft Fabric and Power BI |
| **Data** | The pricing calculator's enterprise BI template, and Microsoft's sample data in the labs: an AdventureWorks product database, product files and New York taxi trips |
| **Bootcamp week** | Week 5 (October 2026), Level 3 Data Technician Skills Bootcamp, Leep Talent |
| **Type** | Individual research and scenario work, plus guided labs from Microsoft's DP-900 course, "Introduction to Microsoft Azure Data" |

## 💡 Skills demonstrated

**✔️ Cloud computing fundamentals**
- Service models (IaaS, PaaS, SaaS) and deployment models (public, private, hybrid, community)
- The business case for cloud: lower upfront cost, scaling, speed, reliability and tools on demand, against running everything on premises
- Comparing AWS, Azure and Google Cloud

**✔️ Costing and consulting**
- Producing and reading a cost estimate in the Azure Pricing Calculator
- Turning a client's requirements into a recommendation with costs, benefits and risks (DataCore Enterprises)
- Weighing control against cost and responsibility, as in the shared responsibility model

**✔️ Azure data services (guided labs)**
- Relational data in Azure SQL Database
- Non-relational files and documents in Azure Storage (Blob storage, Data Lake Storage Gen2 and Azure Files) and Azure Cosmos DB
- Analytical data in a Microsoft Fabric lakehouse, and real-time ingestion with an eventstream and eventhouse
- Querying across these services with SQL and KQL

**✔️ Law and compliance**
- Explaining UK computer misuse, data protection and copyright law in plain language, with a practical example of each

## 📗 Exercises covered

| Task | What I did |
|---|---|
| Cloud research | Explained the service and deployment models, the benefits of cloud and the three main providers |
| Cost estimate | Priced the "Design an enterprise BI solution" template in the Azure Pricing Calculator |
| Client scenario | Recommended a service model for DataCore Enterprises, with costs, benefits and risks |
| Azure services | Researched Azure Data Factory, Microsoft Entra ID and Application Insights |
| DP-900 labs | Six guided labs across SQL Database, Storage, Cosmos DB, Fabric and Power BI |
| UK law | Summarised the main Acts on computer use and data, and matched 13 legal statements to seven Acts |

### Service models

| Model | Provider manages | Customer manages | Example |
|---|---|---|---|
| IaaS | Physical hardware, networking, virtualisation | Operating system, software, applications, data | Azure Virtual Machines |
| PaaS | All of the above, plus the operating system, runtime and development tools | Their own applications and data | Azure SQL Database, Azure App Service |
| SaaS | Everything, including updates and security | Only their own use of it | Microsoft 365, Salesforce |

### Deployment models

| Model | Suits | Example |
|---|---|---|
| Public | Low upfront cost and quick scaling | An online shop renting extra capacity for Black Friday, or Netflix running its back-end systems on AWS |
| Private | Sensitive data, strict regulation and steady demand | A bank storing customer accounts and transactions |
| Hybrid | A mix of sensitive and everyday work, or a gradual move to the cloud | A bank keeping accounts private while running its mobile app in the public cloud |
| Community | Organisations in one sector with shared rules | NHS trusts sharing a platform for patient records |

AWS has the widest range of services. Azure integrates closely with Microsoft 365, Teams and Power BI and suits hybrid set-ups. Google Cloud is the smallest of the three but growing fastest.

## 💷 Cost estimate: enterprise BI solution

![Azure Pricing Calculator estimate](images/azure-pricing-calculator-estimate.png)

| | GBP | USD |
|---|---:|---:|
| Upfront cost | £0.00 | |
| Estimated monthly cost | £5,886.44 | $7,799.23 |
| Estimated annual cost | £70,637.24 | $93,590.81 |

The template prices a pipeline that moves data from an on-premises data warehouse to the cloud and serves it through a BI model.

## 🏭 DataCore Enterprises: recommendation

DataCore is a large company with its own IT staff. It wants to move its internal database servers to the cloud and keep full control of operating systems and storage, so I recommended **IaaS**: the provider runs the hardware, networking and virtualisation, and DataCore manages everything above that.

- **Cost:** use the Azure Pricing Calculator and compare the estimate with the total cost of running the current servers.
- **Benefits:** no hardware to buy, scaling with demand, backup across regions, less maintenance and built-in security tools.
- **Risks:** pay-as-you-go costs that grow unless usage is monitored, DataCore still securing its own systems and data, UK GDPR rules on where data is held, and an internet outage making databases unavailable.

## 🔧 Azure services researched

| Service | What it does |
|---|---|
| Azure Data Factory | Moves data between systems and transforms it on the way, using pipelines. It has more than 90 built-in connectors. |
| Microsoft Entra ID | Cloud identity and access management, renamed from Azure Active Directory in 2023, with single sign-on and multi-factor authentication |
| Application Insights | Part of Azure Monitor. It tracks live web applications, with dashboards, alerts and queries written in KQL. |

I also suggested Azure Machine Learning for a café chain: forecasting busy days from past sales to plan staffing and stock and cut food waste.

## 🧪 Guided labs (DP-900)

| Lab | Type of data | What the lab covers |
|---|---|---|
| Explore Azure SQL Database | Relational | Creating a database with the AdventureWorks sample and querying its product tables |
| Explore Azure Storage (part 1) | Non-relational files | A storage account, a blob container for JSON product files, Data Lake Storage Gen2 folders and an Azure Files share |
| Explore Azure Storage (part 2) | Non-relational documents | An Azure Cosmos DB account, adding an item as JSON and querying the items |
| Explore data analytics in Microsoft Fabric | Analytical | A Fabric lakehouse, loading New York taxi trips into a table and querying it through the SQL analytics endpoint |
| Explore real-time analytics in Microsoft Fabric | Streaming | An eventstream feeding a live taxi data stream into an eventhouse, queried with KQL |
| Explore fundamentals of data visualisation | Reporting | A simple report from sample data in Power BI |

My workbook's evidence for the labs is the completion screens. For SQL I wrote myself, see my [SQL repository](https://github.com/isobel-hannington/sql-northwind-world-analysis).

## 🔒 Handling data responsibly

| Law | Key points |
|---|---|
| Computer Misuse Act 1990 | Section 1: unauthorised access, such as guessing a colleague's password. Section 2: access with intent to commit a further crime. Section 3: acts that impair a computer, such as planting ransomware. |
| Police and Justice Act 2006 | Made it an offence to make, supply or obtain hacking tools for use in an offence, covered denial-of-service attacks and raised maximum sentences |
| Data Protection Act 2018 and UK GDPR | Personal data must be used for specified purposes, kept accurate and not kept longer than necessary. Sensitive data, such as health or religion, needs the employee's permission. |
| Copyright, Designs and Patents Act 1988 | Covers copying and sharing protected work, such as using a song in a video without permission |

Of the 13 legal statements I matched, one wasn't illegal: creating or using a hacking tool for authorised penetration testing.

## 🎓 Key learning outcomes

- **The cloud swaps an upfront cost for a running one.** The estimate needs no upfront spend, but about £70,600 a year has to be budgeted and monitored.
- **Moving to the cloud doesn't hand over every responsibility.** Under IaaS, the customer still secures its own operating systems, data and access.
- **The same SQL ideas travel.** `SELECT`, `WHERE`, `JOIN` and `GROUP BY` work across a relational database, a document database and a lakehouse.

## 🧠 What I'd change

My workbook shows my original answers. Three needed correcting, and this page shows the corrected versions:

- **IaaS, the right way round.** My first definition said the provider maintains the operating system, software and data. Under IaaS, the customer manages those.
- **Copy figures from the source.** I typed the monthly estimate as £5,836.44, but the calculator shows £5,886.44, which matches the annual total.
- **Check examples in detail.** Netflix runs its back-end systems on AWS, but its video is delivered through its own network, not streamed from AWS.

## 🛠️ Tools and technologies

- **Azure Pricing Calculator:** the enterprise BI cost estimate
- **Azure SQL Database, Azure Storage and Azure Cosmos DB:** relational and non-relational data in the labs
- **Microsoft Fabric:** the lakehouse, eventstream and eventhouse labs
- **Power BI:** the data visualisation lab

## 📁 Repository contents

| File or folder | What it is |
|---|---|
| `Data_Technician_Workbook_Week_5.docx` | The Leep Talent Week 5 workbook with my answers and lab evidence |
| `images/` | Screenshot of the Azure Pricing Calculator estimate |
