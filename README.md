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



