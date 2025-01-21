# azure_services_det

https://techcommunity.microsoft.com/t5/ai-azure-ai-services-blog/advanced-rag-with-azure-ai-search-and-llamaindex/ba-p/4115007
Services Every Cloud Developer Should Know About!

Awesome Azure — Top Azure Services Every Developer Must Know
TL;DR:
Azure PaaS Services allow you to avoid the expense and complexity of buying and managing software licenses, underlying application infrastructure and middleware, container orchestrators, or other resources. You manage the applications and services you develop, and Azure manages everything else.
PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. Cloud features such as scalability, high availability, and multi-tenant capability are included, reducing the amount of coding that developers must do. PaaS provides all of the capabilities that you need to support the complete web application lifecycle: building, testing, deploying, managing, and updating within the same integrated environment.
Below is the Curated List of Top Microsoft Azure PaaS/Serverless Services:

Azure App Service
Azure App Service is a fully managed web application hosting platform. It allows you to focus on designing and building your app while Azure takes care of the infrastructure to run and scale your applications. It enables you to build and host web applications in the programming language of your choice without managing infrastructure. It is ideal if you don’t need tight control over the hosting infrastructure.
You can also use App Service to deploy a web application based on the Docker image. Hosting your web application using App Service makes deploying and managing a web app much easier when compared to managing physical servers or virtual machines.
With Azure App Service, you can quickly build, deploy, and scale enterprise-grade web, mobile, and API apps in the programming language of your choice (such as .NET Core, .NET Framework, Java, Ruby, Node.js, PHP, and Python) and running on any platform (Linux, Windows). You can meet rigorous performance, scalability, availability, security, and compliance requirements while using a fully managed platform to perform infrastructure maintenance.
Features:
	• Deployment slots (streamline deployment and rollback).
	• Built-in autoscale support.
	• Built-in load balancing and traffic manager provide high availability.
	• Docker support.
	• Advance Telemetry using Application Insights.
	• Continuous integration/deployment support.

Azure App Service Plan
Azure App Service Plan is a set of virtual server resources that run App Service apps. Every App Service app you create must be assigned to a single App Service plan that runs it. A single App Service plan can host multiple App Service web apps. In most cases, the number of apps you can run on a single plan will be limited by the performance characteristics of the apps and the resource limitations of the plan.
App Service plans are the unit of billing (referred to as its SKU or pricing tier) for App Service. It specifies the operating system (Windows or Linux), hardware (memory, CPU, disk storage, and so on), and the availability of services like automatic backup and restore. It determines the performance characteristics of the virtual servers that run the apps assigned to the plan, as well as the App Service features to which those apps have access. The number of web apps deployed to your App Service plans has no effect on your bill.

Azure Functions
Azure Functions is a serverless solution that allows you to write less code, maintain less infrastructure, and save on costs. Instead of worrying about deploying and maintaining servers, the cloud infrastructure provides all the up-to-date resources needed to keep your applications running. Functions can execute code in almost any modern language. You focus on the code that matters most to you, in the most productive language for you, and Azure Functions handles the rest.
Functions are a key component of Azure Serverless computing. Functions scale automatically based on demand, so they’re a solid choice when demand is variable. Azure Functions are a great solution for processing data, integrating systems, working with the IoT, and building simple APIs and microservices. It can be used to achieve decoupling, high throughput, shared, and reusability.
Azure Function is a trigger-based service that supports triggers that enables enterprises to run event-triggered codes without having an infrastructure for its provision. It runs a script or piece of code in response to a variety of events. Developers use Azure Functions to connect to data sources or messaging solutions and react to events. There are other integration and automation services in Azure and they all can solve integration problems and automate business processes. They can all define input, actions, conditions, and output.
Azure Functions Triggers: Service Bus, Queue storage, Blob storage, Event Grid, Event Hubs, IoT Hub, HTTP, Cosmos DB, Azure SQL, Timer, etc.

Azure SQL
Azure SQL Database is a fully managed service that has built-in high availability, backups, and other common maintenance operations. It is a PaaS database engine deployment option of Azure SQL that abstracts both the OS and the SQL Server instance away from users, and handles most of the database management functions, such as upgrading, patching, backups, and monitoring, without user involvement. You don’t have to manage the underlying infrastructure.
SQL Database is also the only deployment option that supports scenarios that require unlimited database storage (hyperscale) and autoscaling for unpredictable workloads (serverless). SQL Database has the industry’s highest availability SLA. SQL Database provides 99.99 percent availability. Azure SQL Database also comes with a firewall so that you can control access to your data.
Service tiers (vCore model): General Purpose, Business Critical, Hyperscale

Azure Cosmos DB
Azure Cosmos DB is a fully managed NoSQL database for modern app development at any scale. It provides a highly scalable store for non-relational data. It takes database administration off your hands with automatic management, updates, and patching. It also handles capacity management with cost-effective serverless and automatic scaling options that respond to application needs to match capacity with demand. It makes it easy to build scalable, highly responsive applications at a global scale.
Azure Cosmos DB is a globally distributed, multi-model database service that enables you to elastically and independently scale throughput and storage across any number of Azure regions worldwide. It provides comprehensive SLA for throughput, latency, availability, and consistency guarantees. You can take advantage of fast, single-digit millisecond data access by using any one of several popular APIs.
Azure Cosmos DB offers multiple database APIs:
	• NoSQL (document format, native to Azure Cosmos DB)
	• MongoDB (document structure, via BSON format)
	• Cassandra (columnar format, column-oriented schema)
	• Gremlin (graph format, queries and stores data as edges and vertices.)
	• Table (key/value format)
	• *PostgreSQL (PostgreSQL at any scale, with the Citus open-source superpower of distributed tables)
Use Cases: Azure Cosmos DB is well-suited for IoT, gaming, retail, and operational logging applications. A common design pattern in these applications is to use changes to the data to trigger additional actions. Azure Cosmos DB enables you to build highly responsive and Always On applications to support constantly changing data.

Azure Blob Storage
Azure Blob Storage (known as object storage or container storage) is an object storage solution for the cloud. It is optimized for storing massive amounts of unstructured data, meaning that there are no restrictions on the kinds of data it can hold, such as text or binary data. Blobs aren’t limited to common file formats. A blob could contain gigabytes of binary data streamed from a scientific instrument, an encrypted message for another application, or data in a custom format for an app you’re developing.
Azure Storage provides different options for accessing block blob data based on usage patterns. Each access tier in Azure Storage is optimized for a particular pattern of data usage. The available access tiers: Hot, Cool, Archive.
Use Cases:
	• Serving images or documents directly to a browser.
	• Storing files for distributed access.
	• Streaming video and audio.
	• Writing to log files.
	• Storing data for backup and restore, disaster recovery, and archiving.
	• Storing data for analysis by an on-premises or Azure-hosted service.

Azure Service Bus
Azure Service Bus is a fully managed enterprise integration message broker. It enables you to decouple applications and services from each other. Data is transferred between different applications and services using messages. It allows you to build applications that take advantage of asynchronous messaging patterns to broker messages between producers and consumers, along with structured FIFO messaging and publish/subscribe capabilities with complex routing.
Azure Service Bus can exchange messages in two different ways:
Azure Service Bus Queue: It is a simple temporary storage location for messages. A sending component adds a message to the queue. A destination component picks up the message at the front of the queue. Each message is received by only one receiver.
Azure Service Bus Topic: It is similar to a queue, but a topic can have multiple subscriptions. This means that multiple destination components can subscribe to a specific topic, so each message is delivered to multiple receivers. Subscriptions can also filter the messages in the topic to receive only messages that are relevant.
Use a topic if you want a single message to be delivered to more than one destination component (1-N). Otherwise, use a Service Bus queue for 1–1 communication.
Difference between Azure Service Bus Queues and Topics
Azure Functions integrates with Azure Service Bus via triggers and bindings. Use the Service Bus trigger to respond to messages from a Service Bus queue or topic.

Azure Queue Storage
Azure Queue Storage is a managed cloud messaging service that stores large numbers of messages. Azure Queue Storage implements cloud-based queues to enable asynchronous communication between components of a distributed application, so they can scale independently. Each queue maintains a list of messages to be processed asynchronously that can be added by a sender component and processed by a receiver component. Queues let your application scale automatically and immediately when demand changes.
A single queue message can be up to 64 KB in size, and a queue can contain millions of messages, up to the total capacity limit of a storage account. You access messages from anywhere in the world via authenticated calls using HTTP or HTTPS. Queue storage is often used to create a backlog of work to process asynchronously.
Use Cases:
	• Decouple components
	• Build resilience
	• Build process workflows
Queue storage trigger runs an Azure Function as messages are added to Queue. Use a queue trigger to start a function when a new message is received on a queue.
Storage queues are simpler to use, but they’re less sophisticated and less flexible than Service Bus queues.
Difference between Azure Storage Queue and Service Bus Queue

Azure Cache for Redis
Azure Cache for Redis enables you to implement Redis as a fully managed service. It provides an in-memory data store based on the Redis software. It offers both the Redis open-source (OSS Redis) and a commercial product from Redis Inc.
Azure Cache for Redis brings a critical low-latency and high-throughput and secure data storage solution to modern applications. This can help improve the performance and scalability of an application that uses backend data stores heavily. Combining Redis with back-end databases enables you to significantly improve your apps’ performance. You can copy frequently accessed data and store it in memory.
Use Cases:
	• Distributed cache
	• Content cache
	• Session store
	• Message broker
	• Distributed transactions
	• Cloud migration
Service tiers: Basic, Standard, Premium, Enterprise, Enterprise Flash

Azure Key Vault
Azure Key Vault is a centralized cloud service for securely storing and accessing an application’s secrets in a single, central location. A secret is anything that you want to tightly control access to, such as API keys, passwords, encryption keys, server-side tokens, certificates, or cryptographic keys. It provides secure access to sensitive information by providing access control and logging capabilities.
Three primary concepts used in Azure Key Vault: vaults, keys, and secrets.
Containers types: Vaults and Hardware security module (HSM) pools.
Benefits:
	• Centralized application secrets
	• Simplified administration of application secrets
	• Securely stored secrets and keys
	• Access monitoring and access control
	• Integration with other Azure services
Azure Key Vault Overview

Azure App Configuration
Azure App Configuration is a service to centrally manage and secure your configuration settings, and to manage app features. Modern applications, generally have many components that are distributed in nature. Spreading configuration settings across these components can lead to hard-to-troubleshoot errors. Use App Configuration to store all the settings for your application and secure their accesses in one place. App Configuration complements Azure Key Vault, which is used to store application secrets.
Use Cases:
	• Centralize management and distribution of hierarchical configuration data for different environments and geographies.
	• Dynamically change application settings without the need to redeploy or restart an application.
	• Control feature availability in real-time.
	• Microservices based on Azure Kubernetes Service, Azure Service Fabric, or other containerized apps deployed in one or more geographies.
	• Serverless apps, which include Azure Functions or other event-driven stateless compute apps.
	• Continuous deployment pipeline.
Benefits:
	• easy setup, can be set up in minutes.
	• Flexible key representations and mappings.
	• Tagging with labels.
	• Point-in-time replay of settings.
	• Dedicated UI for feature flag management.
	• Comparison of two sets of configurations on custom-defined dimensions.
	• Enhanced security through Azure-managed identities.
	• Complete data encryptions, at rest or in transit.
	• Native integration with popular frameworks.
Azure App Configuration Overview

Azure CDN
Azure Content Delivery Network (Azure CDN) is Azure’s content delivery network. It is a distributed network of servers that is used to cache and store content. These servers are in locations (known as point-of-presence (POP)) that are close to end users to minimize latency. It can help reduce latency and improve performance for high-bandwidth content. Azure CDN allows an organization to deliver content that requires significant bandwidth with a minimum amount of latency to clients all across the world.
Benefits:
	• Better performance and a smoother user experience with large or streamed files.
	• Improved results with applications that require multiple round trips to display content.
	• Greater scaling, especially with rapidly spiking loads, such as global launch events.
	• Reduced traffic to the origin server.

Azure Application Insights
Application Insights is an extension of Azure Monitor and provides Application Performance Monitoring (APM) features. Application Insights automatically gathers information related to performance, errors, and exceptions in applications. You also use Application Insights to diagnose what has caused the problems that affect an application.
Features:
	• Smart Detection — automatic failure and anomaly detection through proactive telemetry analysis.
	• Distributed Tracing — allows searching for and visualizing an end-to-end flow of a given execution or transaction.
	• Usage — understand which features are popular with users and how users interact and use your application.
	• Live Metrics — real time with no effect on the host environment.
	• Availability — to test the overall availability and responsiveness over time.
	• GitHub or Azure DevOps integration.

Azure Monitor
Azure Monitor is a comprehensive monitoring solution for collecting, analyzing, and responding to telemetry from your cloud and on-premises environments. IT Operations, DevOps, and Developer teams can use Azure Monitor to maximize the availability and performance of applications and services. Azure Monitor is a key resource to keep watch on how all your Azure resources are performing, and to trigger alerts if there is any sort of problem.
Azure Monitor provides features and capabilities in three areas:
	• Monitor and visualize metrics
	• Query and analyze logs
	• Set up alerts and actions

Azure Cognitive Search (formerly known as “Azure Search”)
Azure Cognitive Search (formerly known as “Azure Search”) provides a cloud-based solution for indexing and querying a wide range of data sources, and creating comprehensive and high-scale search solutions. It provides the infrastructure, APIs, and tools to build rich search solutions that extract data from various structured, semi-structured, and non-structured documents for enterprise applications.
Azure Cognitive Search offers a rich query language to support a broad range of scenarios, from free text search, to highly-specified query patterns. With Azure Cognitive Search, you can:
	• Index documents and data from a range of sources.
	• Use cognitive skills to enrich index data.
	• Store extracted insights in a knowledge store for analysis and integration.


From <https://medium.com/awesome-azure/azure-most-useful-azure-services-every-developer-must-know-top-azure-paas-serverless-services-developer-c55b829ac6d7> 

![image](https://github.com/user-attachments/assets/78061f7b-f335-43b4-9d33-cb10d4d70838)




Service	Description
Anomaly Detector	Easily add anomaly detection capabilities to your apps.
Azure Bot Service	Intelligent, serverless bot services that scale on demand
Azure Cognitive Search	AI-powered cloud search service for mobile and web app development
Azure Databricks	Fast, easy, and collaborative Apache Spark-based analytics platform
Azure Machine Learning	Bring AI to everyone with an end-to-end, scalable, trusted platform with experimentation and model management
Azure Open Datasets	Cloud platform to host and share curated open datasets to accelerate the development of machine learning models
Azure Cognitive Services	Deploy high-quality AI models as APIs
Azure Video Analyzer	An AI service for quickly building video analytics solutions
Computer Vision	Distill actionable information from images
Content Moderator	Automated image, text, and video moderation
Custom Vision	Easily customize your own state-of-the-art computer vision models for your unique use case
Data Science Virtual Machines	Rich pre-configured environment for AI development
Face API	Detect, identify, analyze, organize, and tag faces in photos
Azure Form Recogniser	The AI-powered document extraction service that understands your forms
Azure Immersive Reader	Empower users of all ages and abilities to read and comprehend text
Kinect DK	Build computer vision and speech models using a developer kit with advanced AI sensors
Language Understanding	Teach your apps to understand commands from your users
Microsoft Genomics	Power genome sequencing & research insights
Personalizer	An AI service that delivers a personalized user experience
Project Bonsai	A machine teaching service for creating intelligent industrial control systems using simulations
QnA Maker	Distill information into conversational, easy-to-navigate answers
Speaker Recognition	A Speech service feature that verifies and identifies speakers
Speech to Text	A Speech service feature that accurately converts spoken audio to text
Speech Translation	Easily integrate real-time speech translation intoyour app
Text Analytics	Easily evaluate sentiment and topics to understand what users want
Text to Speech	A Speech service feature that converts text to lifelike speech
Translator	Easily conduct machine translation with a simple REST API call
Azure Metrics Advisor	An AI service that monitors metrics and diagnoses issues
Health Bot	A managed service purpose-built for the development of virtual healthcare assistants
Azure Percept	Accelerate edge intelligence from silicon to service
Azure Applied AI Services	Specialized services that enable organizations to accelerate time to value in applying AI to solve common scenarios
 
Analytics – Collect, process, store, analyze, and visualize data irrespective of its volume and variety
Service	Description
Azure Analysis Services	Enterprise-grade analytics engine as a service
Azure Data Explorer	Fast and highly scalable data exploration service
Azure Data Lake Storage	Massively scalable, secure data lake functionality built on Azure Blob Storage
Azure Data Share	A simple and safe service for sharing big data with external organizations
Azure Databricks	Fast, easy, and collaborative Apache Spark-based analytics platform
Azure Stream Analytics	Real-time analytics on fast-moving streams of data from applications and devices
Azure Synapse Analytics	Limitless analytics service with unmatched time to insight
Data Catalog	Get more value from your enterprise data assets
Azure Data Factory	Hybrid data integration at enterprise scale made easy
Data Lake Analytics	Distributed analytics service that makes big data easy
Event Hubs	Receive telemetry from millions of devices
HDInsight	Provision cloud Hadoop, Spark, R Server, HBase, and Storm clusters
Power BI Embedded	Embed fully interactive, stunning data visualizations in your applications
R Server for HDInsight	Predictive analytics, machine learning, and statistical modeling for big data
Azure Purview	Maximize business value with unified data governance
Microsoft Graph Data Connect	A secure, high-throughput connector designed to copy select Microsoft 365 productivity datasets into your Azure tenant
 
Azure Virtual Desktop – The best virtual desktop experience through Azure
Service	Description
Azure Virtual Desktop	The best virtual desktop experience, delivered on Azure
VMware Horizon Cloud on Microsoft Azure	Provision Windows desktops and apps with VMware and Azure Virtual Desktop
Citrix Virtual Apps and Desktops for Azure	Provision Windows desktops and apps on Azure with Citrix and Azure Virtual Desktop
 
Blockchain – Get integrated tools to build and manage blockchain-based applications
Service	Description
Azure Blockchain Service	Build, govern, and expand consortium blockchain networks
Azure Blockchain Workbench	Easily prototype blockchain apps in the cloud
Azure Cosmos DB	Fast NoSQL database with open APIs for any scale
Azure Logic Apps	Automate the access and use of data across clouds without writing code
Microsoft Azure Confidential Ledger	Easily use a REST API managed service to store your unstructured metadata in a blockchain structure
 
Compute – Avail cloud computing services and scale at your wish while paying only for the resources that you use
Service	Description
API Apps	Easily build and consume Cloud APIs
App Service	Quickly create powerful cloud apps for web and mobile
Azure CycleCloud	Create, manage, operate, and optimize HPC and big compute clusters of any scale
Azure Functions	Process events with serverless code
Azure Kubernetes Service (AKS)	Simplify the deployment, management, and operations of Kubernetes
Azure Quantum	Experience quantum impact today on Azure
Azure Spot Virtual Machines	Provision unused compute capacity at deep discounts to run interruptible workloads
Azure Spring Cloud	A fully managed Spring Cloud service, jointly built and operated with VMware
Azure VMware Solution	Run your VMware workloads natively on Azure
Batch	Cloud-scale job scheduling and compute management
Cloud Services	Create highly available, infinitely-scalable cloud applications and APIs
Container Instances	Easily run containers on Azure without managing servers
Linux Virtual Machines	Provision virtual machines for Ubuntu, Red Hat, and more
Mobile Apps	Build and host the backend for any mobile app
Service Fabric	Develop microservices and orchestrate containers on Windows or Linux
SQL Server on Virtual Machines	Host enterprise SQL Server apps in the cloud
Static Web Apps	A modern web app service that offers streamlined full-stack development from source code to global high availability
Virtual Machine Scale Sets	Manage and scale up to thousands of Linux and Windows virtual machines
Virtual Machines	Provision Windows and Linux virtual machines in seconds
Web Apps	Quickly create and deploy mission-critical web apps at scale
Azure Virtual Desktop	The best virtual desktop experience, delivered on Azure
Azure Dedicated Host	A dedicated physical server to host your Azure VMs for Windows and Linux
Azure VM Image Builder	Simplify your image building process with easy to use tool
 
Containers – Integrated tools to develop and manage all the applications faster within a container
Service	Description
API Apps	Easily build and consume Cloud APIs
Azure Functions	Process events with serverless code
Azure Kubernetes Service (AKS)	Simplify the deployment, management, and operations of Kubernetes
Azure Red Hat OpenShift	Fully managed OpenShift service, jointly operated with Red Hat
Container Instances	Easily run containers on Azure without managing servers
Container Registry	Store and manage container images across all types of Azure deployments
Mobile Apps	Build and host the backend for any mobile app
Service Fabric	Develop microservices and orchestrate containers on Windows or Linux
Web App for Containers	Easily deploy and run containerized web apps that scale with your business
Web Apps	Quickly create and deploy mission-critical web apps at scale
 
Databases – With fully managed and secure database services, innovate faster and grow rapidly
Service	Description
Azure API for FHIR	Easily create and deploy an FHIR service for health data solutions and interoperability
Azure Cache for Redis	Accelerate applications with high-throughput, low-latency data caching
Azure Cosmos DB	Fast NoSQL database with open APIs for any scale
Azure Database for MariaDB	Managed MariaDB database service for app developers
Azure Database for MySQL	Fully managed, scalable MySQL Database
Azure Database for PostgreSQL	Fully managed, intelligent, and scalable PostgreSQL
Azure Database Migration Service	Simplify on-premises database migration to the cloud
Azure SQL	Managed, always up-to-date SQL instance in the cloud
Azure SQL Database	Managed, intelligent SQL in the cloud
Azure SQL Edge	Consume Services privately on Azure Platform
Azure SQL Managed Instance	Managed, always up-to-date SQL instance in the cloud
SQL Server on Virtual Machines	Host enterprise SQL Server apps in the cloud
Table Storage	NoSQL key-value store using semi-structured datasets
Azure Managed Instance for Apache Cassandra	Cloud Cassandra with flexibility, control, and scale
 
Developer Tools – Tools to create and manage cloud applications on any platform and in any language
Service	Description
App Configuration	Fast, scalable parameter storage for app configuration
Azure DevOps	Services for teams to share code, track work, and ship software
Azure DevTest Labs	Quickly create environments using reusable templates and artifacts
Azure Lab Services	Set up labs for classrooms, trials, development and testing, and other scenarios
Azure Pipelines	Continuously build, test, and deploy to any platform and cloud
SDKs	Get the SDKs and command-line tools you need
Visual Studio	The powerful and flexible environment for developing applications in the cloud
Visual Studio Code	A powerful, lightweight code editor for cloud development
 
DevOps – Innovative tools for faster and reliable tools
Service	Description
Azure Artifacts	Create, host, and share packages with your team
Azure Boards	Plan, track, and discuss work across your teams
Azure DevOps	Services for teams to share code, track work, and ship software
Azure DevTest Labs	Quickly create environments using reusable templates and artifacts
Azure Monitor	Full observability into your applications, infrastructure, and network
Azure Pipelines	Continuously build, test, and deploy to any platform and cloud
Azure Repos	Get unlimited, cloud-hosted private Git repos for your project
Azure Test Plans	Test and ship with confidence with a manual and exploratory testing toolkit
DevOps tool integrations	Use your favorite DevOps tools with Azure
 
Hybrid + Multicloud – Incorporate the Azure agility of cloud computing into the operations at your workplace
Service	Description
Azure Active Directory	Synchronize on-premises directories and enable single sign-on
Azure Arc	Extend Azure management and services anywhere
Azure Database for PostgreSQL	Fully managed, intelligent, and scalable PostgreSQL
Azure DevOps	Services for teams to share code, track work, and ship software
Azure ExpressRoute	Dedicated private network fiber connections to Azure
Azure IoT Edge	Extend cloud intelligence and analytics to edge devices managed by Azure IoT Hub
Azure Sentinel	Put cloud-native SIEM and intelligent security analytics to work to help protect your enterprise
Azure SQL Database	Managed, intelligent SQL in the cloud
Azure SQL Edge	Consume Services privately on Azure Platform
Azure Stack	Build and run innovative hybrid applications across cloud boundaries
Security Center	Unify security management and enable advanced threat protection across hybrid cloud workloads
Azure Stack HCI	Run your production workloads on hybrid, familiar hyper-converged infrastructure
Azure Stack Hub	Azure Stack Hub is sold as an integrated hardware system, with software pre-installed on validated hardware
Azure Stack Edge	An Azure managed device that brings the compute, storage, and intelligence of Azure to the edge
Azure Modular Datacenter	A complete, rugged data center solution
 
Identity – Increase security by managing user identities and protecting them against advanced threats across applications, data, infrastructure, and devices
Service	Description
Azure Active Directory	Synchronize on-premises directories and enable single sign-on
Azure Active Directory Domain Services	Join Azure virtual machines to a domain without domain controllers
Azure Information Protection	Better protect your sensitive information—anytime, anywhere
Azure Active Directory External Identities	Consumer identity and access management in the cloud
 
Integration – Seamless integration between cloud-based applications and on-premise software across the enterprise
Service	Description
API Management	Publish APIs to developers, partners, and employees securely and at scale
Azure API for FHIR	Easily create and deploy an FHIR service for health data solutions and interoperability
Event Grid	Reliable event delivery at a massive scale
Azure Logic Apps	Automate the access and use of data across clouds without writing code
Service Bus	Connect across private and public cloud environments
Azure Web PubSub	Easily build real-time messaging web applications using WebSockets and the publish-subscribe pattern
 
Internet of Things – Without changing your infrastructure, enjoy the perks of IoT on all applications
Service	Description
API Management	Publish APIs to developers, partners, and employees securely and at scale
Azure Cosmos DB	Fast NoSQL database with open APIs for any scale
Azure Digital Twins	Build next-generation IoT solutions that model entire environments in real-time
Azure Functions	Process events with serverless code
Azure IoT Central	Accelerate the creation of IoT solutions
Azure IoT Edge	Extend cloud intelligence and analytics to edge devices managed by Azure IoT Hub
Azure IoT Hub	Connect, monitor, and manage IoT assets with a scalable platform
Azure IoT solution accelerators	Create fully customizable solutions with templates for common IoT scenarios
Azure Machine Learning	Bring AI to everyone with an end-to-end, scalable, trusted platform with experimentation and model management
Azure Maps	Simple and secure location APIs provide geospatial context to data
Azure RTOS	Making embedded IoT development and connectivity easy
Azure Sphere	Securely connect embedded MCU-powered devices from silicon to cloud
Azure SQL Edge	Consume Services privately on Azure Platform
Azure Stream Analytics	Real-time analytics on fast-moving streams of data from applications and devices
Azure Time Series Insights	Monitor, analyze, and visualize your industrial IoT data at scale
Event Grid	Reliable event delivery at a massive scale
Kinect DK	Build computer vision and speech models using a developer kit with advanced AI sensors
Azure Logic Apps	Automate the access and use of data across clouds without writing code
Notification Hubs	Send push notifications to any platform from any back end
Windows 10 IoT Core Services	Long-term OS support and services to manage device updates and assess device health
Azure Defender for IoT	Monitor and detect security threats to both managed and unmanaged IoT assets
Azure Percept	Accelerate edge intelligence from silicon to service
Windows IoT Enterprise	Build intelligent edge solutions with world-class developer tools, long-term support, and enterprise-grade security.
 
Management and Governance – Automate and optimize all your cloud resources with simplified management and compliance
Service	Description
Automation	Simplify cloud management with process automation
Azure Advisor	Your personalized Azure best practices recommendation engine
Azure Backup	Simplify data protection and protect against ransomware
Azure Blueprints	Enabling quick, repeatable creation of governed environments
Azure Lighthouse	Empowering service providers to manage customers at scale and with precision
Azure Managed Applications	Simplify management of cloud offerings
Azure Migrate	Easily discover, assess, right-size, and migrate your on-premises VMs to Azure
Azure mobile app	Stay connected to your Azure resources—anytime, anywhere
Azure Monitor	Full observability into your applications, infrastructure, and network
Azure Policy	Implement corporate governance and standards at scale for Azure resources
Azure Resource Manager	Simplify how you manage your app resources
Azure Resource Manager templates	Deliver infrastructure as code for all your Azure resources using Resource Manager
Azure Service Health	Personalized guidance and support for when issues in Azure services affect you
Azure Site Recovery	Keep your business running with built-in disaster recovery service
Cloud Shell	Streamline Azure administration with a browser-based shell
Azure Cost Management and Billing	Manage your cloud spending with confidence
Microsoft Azure portal	Build, manage, and monitor all Azure products in a single, unified console
Network Watcher	Network performance monitoring and diagnostics solution
Traffic Manager	Route incoming traffic for high performance and availability
Azure Automanage	Simplify and optimize IT management with automated operations
Azure Resource Mover	Simplify how you move multiple resources between Azure regions
Azure Purview	Maximize business value with unified data governance
 
Media – High-quality video content available across devices at any time
Service	Description
Azure Media Player	A single-player for all your playback needs
Content Delivery Network	Ensure secure, reliable content delivery with a broad global reach
Content Protection	Securely deliver content using AES, PlayReady, Widevine, and Fairplay
Encoding	Studio-grade encoding at cloud scale
Live and On-Demand Streaming	Deliver content to virtually all devices with scale to meet business needs
Media Services	Encode, store, and stream video and audio at scale
 
Migration – Easily migrate all your application data to the cloud with required tools, resources, and guide
Service	Description
Azure Database Migration Service	Simplify on-premises database migration to the cloud
Azure Migrate	Easily discover, assess, right-size, and migrate your on-premises VMs to Azure
Azure Site Recovery	Keep your business running with built-in disaster recovery service
Azure Cost Management and Billing	Manage your cloud spending with confidence
Azure Data Box	Appliances and solutions for offline data transfer to Azure​
 
Mixed Reality – Create immersive and collaborative experience by blending both the digital and physical worlds
Service	Description
Azure Digital Twins	Build next-generation IoT solutions that model entire environments in real-time
Kinect DK	Build computer vision and speech models using a developer kit with advanced AI sensors
Azure Remote Rendering	Render high-quality, interactive 3D content, and stream it to your devices in real-time
Spatial Anchors	Create multi-user, spatially aware mixed reality experiences
Object Anchors	Automatically align and anchor 3D content to objects in the physical world
 
Mobile – Build and deploy cross-platform and apps for all mobile devices
Service	Description
API Management	Publish APIs to developers, partners, and employees securely and at scale
App Service	Quickly create powerful cloud apps for web and mobile
Azure Cognitive Search	AI-powered cloud search service for mobile and web app development
Azure Maps	Simple and secure location APIs provide geospatial context to data
Azure Cognitive Services	Deploy high-quality AI models as APIs
Notification Hubs	Send push notifications to any platform from any back end
Spatial Anchors	Create multi-user, spatially aware mixed reality experiences
Visual Studio App Centre	Continuously build, test, release, and monitor your mobile and desktop apps
Xamarin	Create cloud-powered mobile apps faster
Azure Communication Services	Build rich communication experiences with the same secure CPaaS platform used by Microsoft Teams
 
Networking – Bring the best user experience to your customers by connecting on-premise and cloud infrastructure
Service	Description
Application Gateway	Build secure, scalable, and highly available web front ends in Azure
Azure Bastion	Private and fully managed RDP and SSH access to your virtual machines
Azure DDoS Protection	Protect your applications from Distributed Denial of Service (DDoS) attacks
Azure DNS	Host your DNS domain in Azure
Azure ExpressRoute	Dedicated private network fiber connections to Azure
Azure Firewall	Native firewalling capabilities with built-in high availability, unrestricted cloud scalability, and zero maintenance
Load Balancing	Explore Azure load balancing services and find the best solution for your workloads using an easy-to-use service selection tool
Azure Firewall Manager	Central network security policy and route management for globally distributed, software-defined perimeters
Azure Front Door	Secure, fast, and reliable cloud CDN with intelligent threat protection
Azure Internet Analyzer	Test how networking infrastructure changes will impact your customers’ performance.
Azure Private Link	Private access to services hosted on the Azure platform, keeping your data on the Microsoft network
Content Delivery Network	Ensure secure, reliable content delivery with a broad global reach
Network Watcher	Network performance monitoring and diagnostics solution
Traffic Manager	Route incoming traffic for high performance and availability
Virtual Network	Provision private networks, optionally connect to on-premises datacenters
Virtual WAN	Optimize and automate branch to branch connectivity through Azure
VPN Gateway	Establish secure, cross-premises connectivity
Web Application Firewall	A cloud-native web application firewall (WAF) service that provides powerful protection for web apps
Azure Orbital	Satellite ground station and scheduling service connected to Azure for fast downlinking of data
Azure Route Server	Enable network appliances to exchange routes dynamically with virtual networks in Azure
 
Security – Keep your enterprise safe from advanced threats across hybrid cloud workloads
Service	Description
Application Gateway	Build secure, scalable, and highly available web front ends in Azure
Azure Active Directory	Synchronize on-premises directories and enable single sign-on
Azure Active Directory Domain Services	Join Azure virtual machines to a domain without domain controllers
Azure Defender	Protect hybrid cloud workloads
Azure DDoS Protection	Protect your applications from Distributed Denial of Service (DDoS) attacks
Azure Dedicated HSM	Manage hardware security modules that you use in the cloud
Azure Front Door	Secure, fast, and reliable cloud CDN with intelligent threat protection
Azure Information Protection	Better protect your sensitive information—anytime, anywhere
Azure Sentinel	Put cloud-native SIEM and intelligent security analytics to work to help protect your enterprise
Key Vault	Safeguard and maintain control of keys and other secrets
Security Center	Unify security management and enable advanced threat protection across hybrid cloud workloads
VPN Gateway	Establish secure, cross-premises connectivity
Web Application Firewall	A cloud-native web application firewall (WAF) service that provides powerful protection for web apps
Azure Defender for IoT	Monitor and detect security threats to both managed and unmanaged IoT assets
Microsoft Azure Attestation	A unified solution for remotely verifying the trustworthiness of a platform and integrity of the binaries running inside it
Microsoft Azure Confidential Ledger	Easily use a REST API managed service to store your unstructured metadata in a blockchain structure
 
Storage – Get a large and highly scalable cloud data storage to keep your apps and workloads
Service	Description
Archive Storage	An industry-leading price point for storing rarely accessed data
Avere vFXT for Azure	Run high-performance, file-based workloads in the cloud
Azure Backup	Simplify data protection and protect against ransomware
Azure Data Lake Storage	Massively scalable, secure data lake functionality built on Azure Blob Storage
Azure Data Share	A simple and safe service for sharing big data with external organizations
Azure Files	Simple, secure, and serverless enterprise-grade cloud file shares
Azure FXT Edge Filer	Hybrid storage optimization solution for HPC environments
Azure HPC Cache	File caching for high-performance computing (HPC)
Azure NetApp Files	Enterprise-grade Azure file shares, powered by NetApp
Azure Blob Storage	Massively scalable and secure object storage
Azure Data Box	Appliances and solutions for offline data transfer to Azure​
Azure Disk Storage	High-performance, highly durable block storage for Azure Virtual Machines
Queue Storage	Effectively scale apps according to traffic
Storage Accounts	Durable, highly available, and massively scalable cloud storage
Storage Explorer	View and interact with Azure Storage resources
StorSimple	Lower costs with an enterprise hybrid cloud storage solution
Microsoft Azure Confidential Ledger	Easily use a REST API managed service to store your unstructured metadata in a blockchain structure
 
Web – Quick build and deploy web applications
Service	Description
API Apps	Easily build and consume Cloud APIs
API Management	Publish APIs to developers, partners, and employees securely and at scale
App Service	Quickly create powerful cloud apps for web and mobile
Azure Cognitive Search	AI-powered cloud search service for mobile and web app development
Azure Maps	Simple and secure location APIs provide geospatial context to data
Azure SignalR Service	Add real-time web functionalities easily
Azure Spring Cloud	A fully managed Spring Cloud service, jointly built and operated with VMware
Content Delivery Network	Ensure secure, reliable content delivery with a broad global reach
Mobile Apps	Build and host the backend for any mobile app
Notification Hubs	Send push notifications to any platform from any back end
Static Web Apps	A modern web app service that offers streamlined full-stack development from source code to global high availability
Web App for Containers	Easily deploy and run containerized web apps that scale with your business
Web Apps	Quickly create and deploy mission-critical web apps at scale
Azure Communication Services	Build rich communication experiences with the same secure CPaaS platform used by Microsoft Teams
Azure Web PubSub	Easily build real-time messaging web applications using WebSockets and the publish-subscribe pattern
Azure Command-Line Interface (CLI)
It is very important to mention Microsoft Azure commands in any Azure cheat sheet. The Azure command-line is the cross-platform command-line tool that can help you manage your resources. You can also develop custom automation with this tool.
You can approach Azure CLI through a selection of Azure Cloud Shell environments in your browser. After installing Azure CLI by following the given instructions, you should also check the version of your Azure CLI by using ‘az version’ command. Once you are done, you need to sign in with ‘az login’ to use the CLI commands with the local install. 
Common Commands
As you start using Microsoft Azure, you will come across several common commands to be implemented in the CLI. Here is an outline of the common command groups:
• ‘az group’ deals with resource groups.
• ‘az VM’ deals with virtual machines.
• ‘az storage account’ deals with storage accounts.
• ‘az keyvault’ deals with the Key Vault.
• ‘az webapp’ deals with Web applications.
• ‘az sql server’ deals with SQL databases.
• ‘az cosmosdb’ command relates to functions of CosmosDB
This organization of CLI commands into groups is also an important part of every Azure cheat sheet. You can choose ‘az find’ to look for more command names.
Arguments Available Globally
The next component of this Azure cheat sheet is the discussion on globally available arguments, that can be used with every command.
• The ‘- -output’ argument helps in changing the output format. The different formats available in this argument include JSON, tsv (tab-separated values), YAML, jsonc (colorized JSON) and table (human-readable ASCII tables). 
• The ‘- -query’ argument helps in filtering the output from Azure services. This argument utilizes the JMESPath query language.
• ‘- -verbose’ argument helps in printing information regarding resources created in Azure in the course of an operation. This argument also provides additional useful information.
• ‘- -debug’ argument is ideal for printing additional information about CLI operations. As the name of the command implies directly, it is ideal for debugging objectives. When users find a bug, they should provide output with ‘- -debug’ tag activated during submission of the bug report. 
Microsoft Azure Certifications
Microsoft offers a plethora of certifications to validate role-based assessment and evaluate the design and implementation skills of the interested candidates. Based on your preference and current knowledge, you can create your own learning path from the beginner level to the expert level. According to the official information by Microsoft, they offer 25 certifications under various specialties for Microsoft Azure. We have compiled a quick list of references for these certifications along with the relevant exams required to undertake.
Certification	Exam	Microsoft Documentation	Whizlabs Course Link
Microsoft 365 Certified: Teams Support Engineer Associate	MS 740	Click Here	Click Here
Azure Administrator Associate(Legacy)	AZ 100,AZ 101(expired),AZ 103(name changed from AZ-103 to AZ-104)	Click Here	Click Here
Azure Developer Associate(Legacy)	AZ 200,AZ 201,AZ 203(expired)	Click Here	Click Here
Azure Solutions Architect Expert(Legacy)	AZ 300(expired),AZ 301(expired), AZ 303(name changed from AZ-303 to AZ-305)	Click Here	Click Here
Azure AI Engineer Associate	AI 102	Click Here	Click Here
Azure Data Engineer Associate	DP 203	Click Here	Click Here
Azure Network Engineer Associate	AZ 700	Click Here	Click Here
Azure Virtual Desktop Specialty	AZ 140	Click Here	Click Here
Azure for SAP Workloads Specialty	AZ 120	Click Here	Click Here
Power Platform Solutions Architect Expert	PL 600	Click Here	Click Here
Azure Data Scientist Associate	DP 100	Click Here	Click Here
Security, Compliance, and Identity Fundamentals	SC 900	Click Here	Click Here
Azure Solutions Architect Expert	AZ 303(name changed from AZ-303 to AZ-305), AZ 304(name changed from AZ-304 to AZ-305)	Click Here	Click Here
Security Operations Analyst Associate	SC 200	Click Here	Click Here
Identity and Access Administrator Associate	SC 300	Click Here	Click Here
Azure Stack Hub Operator Associate	AZ 600	Click Here	Click Here
Azure IoT Developer Specialty	AZ 220	Click Here	Click Here
Azure Developer Associate	AZ 204	Click Here	Click Here
Azure Fundamentals	AZ 900	Click Here	Click Here
DevOps Engineer Expert	AZ 400	Click Here	Click Here
Azure Administrator Associate	AZ 104	Click Here	Click Here
Azure Database Administrator Associate	DP 300	Click Here	Click Here
Azure Security Engineer Associate	AZ 500	Click Here	Click Here
Azure Data Fundamentals	DP 900	Click Here	Click Here






The Azure OpenAI Landing Zone is a reference architecture that integrates a variety of services to create a seamless infrastructure for running OpenAI workloads.
 
	• Azure API Management (APIM)
		○ Provides a unified API gateway for existing back-end services and APIs. It is used in the Landing Zone for managing and securing APIs used by OpenAI applications. APIM can be configured with an Application Gateway as a Web Application Firewall (WAF) to further enhance security. The WAF protects APIs from common web-based attacks like SQL injection or Cross-Site Scripting (XSS) and can be customized to suit specific needs.
		○ Using APIM you can manage and implement policies such as rate throttling and quotas.
	• Azure Web Apps
		○ Provides a fully managed platform for building and hosting web applications. It is used for hosting in a simple way web applications that consume OpenAI services in the Landing Zone.
	• Azure AI services
		○ Offers AI services such as Azure Semantic Search that can be easily integrated into intelligent applications. OpenAI services, being part of Azure AI services, leverage this to deliver advanced language models.
	• Azure Managed Identities
		○ Provides an identity for applications to use when connecting to resources. In the Landing Zone, it allows OpenAI applications to authenticate to any Azure service that supports Azure Active Directory authentication.
		○ OpenAI supports Azure Active Directory (Azure AD) authentication with managed identities for Azure resources. Managed identities for Azure resources can authorize access to Azure AI services resources using Azure AD credentials from applications running in Azure virtual machines (VMs), function apps, virtual machine scale sets, and other services. By using managed identities for Azure resources together with Azure AD authentication, you can avoid storing credentials with your applications that run in the cloud.
	• Azure Application Gateway
		○ An Application Gateway can function as a Web Application Firewall (WAF) providing protection against common web-based attacks. The WAF is configured with a custom set of rules that match the requirements of your OpenAI Applicartion to ensure only authorized access.
	• Azure Private DNS Zones
		○ This service provides name resolution for VMs within a VNet and between VNets. This is important for efficient communication between services in Azure.
	• Azure Private DNS Resolver
		○ In combination with Private DNS Zones, the Azure Private DNS Resolver helps ensure that name resolution for resources in your virtual network is secure and private. This service forwards DNS queries for specific domains to your own DNS servers, enhancing control over DNS results.
The Azure OpenAI Landing Zone integrates all these services to provide a secure and efficient environment for deploying and running OpenAI workloads. This architecture is designed to be scalable, resilient, and customizable to suit the unique needs of your applications.
 
Network and Security
 
Azure provides a robust set of networking and security features that can be used to secure your OpenAI workloads.
 
	• Azure Key Vault
		○ This service safeguards cryptographic keys and secrets used by cloud applications and services. In this architecture, Key Vault stores secrets and keys for the OpenAI service, adding an extra layer of security for sensitive data.
	• Azure Virtual Network (VNet)
		○ Azure Virtual Network enables you to securely connect Azure resources to each other with virtual networks (VNets). A VNet is a representation of your own network in the cloud and you can also connect VNets to your on-premises network.
	• Azure Private Endpoints
		○ Provides secure, private IP address access over a Virtual Network. This is used in the Landing Zone to ensure secure and private connectivity to Azure OpenAI services.
	• Azure Private Link
		○ Azure Private Link provides private connectivity from a virtual network to Azure platform as a service (PaaS), customer-owned, or Microsoft partner services. It simplifies the network architecture and secures the connection between endpoints in Azure by eliminating data exposure to the public internet.
	• Azure Network Security Groups (NSGs)
		○ Network Security Groups (NSGs) are one way to control access and secure your resources in Azure. NSGs act as a firewall, allowing you to define a list of security rules that can allow or deny network traffic to resources.
	• Azure Application Gateway and Web Application Firewall
		○ Azure Application Gateway is a load balancer that enables you to manage traffic to your web applications. The Web Application Firewall (WAF) feature protects your web applications from common web-based attacks like SQL injection and cross-site scripting. The WAF comes pre-configured with protection from many common attacks, but can be customized based on your application's traffic patterns.
	• Azure AI services and Network Security
		○ Azure AI services provides a layered security model. This model enables you to secure your AI services accounts to a specific subset of networks. When network rules are configured, only applications requesting data over the specified set of networks can access the account. You can limit access to your resources with request filtering, allowing only requests originating from specified IP addresses, IP ranges or from a list of subnets in Azure Virtual Networks.
 
Monitoring Azure OpenAI Service
 
When you have critical applications and business processes relying on Azure resources, you want to monitor those resources for their availability, performance, and operation.
 
Azure OpenAI Service collects the same kinds of monitoring data as other Azure resources. Platform metrics and the Activity log are collected and stored automatically, but can be routed to other locations by using a diagnostic setting.
 
Azure Monitor alerts proactively notify you when important conditions are found in your monitoring data. They allow you to identify and address issues in your system before your customers notice them. In the context of Azure Open AI you can proactively analyze and monitor metrics such as Blocked Calls, client errors and others.
 

From <https://techcommunity.microsoft.com/t5/azure-architecture-blog/azure-openai-landing-zone-reference-architecture/ba-p/3882102> 


Security and Privacy details for Azure Open AI

https://techcommunity.microsoft.com/t5/azure-architecture-blog/security-best-practices-for-genai-applications-openai-in-azure/ba-p/4027885


![image](https://github.com/user-attachments/assets/741ac661-1357-473b-a87d-256ff43335b6)


