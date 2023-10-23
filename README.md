## Benie the Bot - Benefits Bot for CalHR

Benie the Bot is a chatbot designed to assist employees with benefits-related inquiries at CalHR (California Department of Human Resources). This repository contains various components of the Benie the Bot system, including a Power Apps package, OpenAI ChatGPT deployment configuration, and instructions for setting up Cognitive Search.

- Table of Contents
- Introduction
- Components
- Features
- Installation
- Documentation
- Contributing
- License

### Architecture
![Architecture](https://github.com/JoseCervantes22/CalHR-ChatBot/assets/133288667/beb83862-8278-450f-8fba-c5e1cbac3ac6)

Components:
- Power Apps Package: This package includes a Power Virtual Agents (PVA) chatbot and a Power Automate API that connects to Azure OpenAI. It allows Benie to interact with users and retrieve responses from the ChatGPT model.

- OpenAI ChatGPT Deployment Configuration: This repository includes the configuration files and scripts required to deploy and manage the ChatGPT model from OpenAI, enabling natural language understanding and conversation with users.

- Cognitive Search: Instructions and resources are provided to set up Cognitive Search, allowing you to index and search the PDF documents provided by CalHR. This feature enhances the bot's ability to retrieve relevant benefits information.

## Features
- Constituent Identification for delivery of personalized information.
- Generation of Constituent analysis to understand user preferences.
- Feedback evaluation with numerical ratings for user satisfaction.
- Guided conversation to help users efficiently.

![new_bytelogo](https://github.com/JoseCervantes22/CalHR-ChatBot/assets/133288667/816ef2ff-ef3e-4d32-84ec-18039c315567)

## Deployment
### Config Azure Open AI - Cognitive search Services
#### Creating a Blob Storage Account: 
1. Navigate to the Azure home page (https://portal.azure.com).
2. In the navigation panel on the left, select "All Services."
3. In the list of services, type "Storage Account".
4. Click "Storage Account" and then select "Create" on the page that opens.
   - Select your subscription.
   - Select your resource group.
   - Type your Storage account name.
   - Select your region.
   - Select Performance (in this case, we will use standard).
   - We select redundancy by default.
   Next steps by default.

![PROYECTO (1)](https://github.com/JoseCervantes22/CalHR-ChatBot/assets/133288667/3ba16ab5-bfdb-4c27-9068-69fa1921f218)

#### Creating a resource in Azure Cognitive Search Service: 
Prerequisite: 
- An azure Subscription
- You should have a comprehension of the data you intend to index. The process of creating an index involves defining a schema, so it's crucial to have a clear idea of which source fields you want to make retrievable and searchable.
- You also need to have a unique field within your source data that can serve as the document key or ID in the index.

1. Navigate to the Azure home page (https://portal.azure.com).
2. In the navigation panel on the left, select "All Services."
3. In the list of services, type "Azure Cognitive Search" in the search bar and select it.
4. On the "Cognitive Search" page, click the "Create" button to begin configuring the resource.
5. Fill in the details in the form:
   - Name: Enter a unique name for your resource.
   - Subscription: Select your Azure subscription.
   - Resource group: Create a new one or select an existing resource group.
   - Location: Choose the geographic region where you want to host the resource.
   - Pricing tier: Select Pricing tier basic.
   - Scale options: Configure the number of search and storage units (this will depend on your scalability requirements).
6. Click on the "Review + create" tab to review the configuration.
7. Once everything is correct, click "Create" to create the resource. Wait for the deployment process to complete.

![PROYECTO (3)](https://github.com/JoseCervantes22/CalHR-ChatBot/assets/133288667/c99d1568-8899-4283-bd9d-4117755076e2)

### Import Data to the Index
When you are prepared to generate the index, utilize a search client capable of transmitting the request. For the purposes of this project, it has been determined that the Azure portal will be the sole method used.
1. Navigate to the your Storage Account in Azure Portal and select.
2. Select upload:

<img src="https://github.com/JoseCervantes22/CalHR-ChatBot/assets/133288667/fe943856-aa07-46e5-85b9-4125af2e0e14" alt="PROYECTO (5)"  width="350" height="80">

3. Select your file CSV Utf and container:

<img src="https://github.com/JoseCervantes22/CalHR-ChatBot/assets/133288667/4e7ea01f-a370-428b-8251-0a61e6616220" alt="PROYECTO (6)" style="width:400px;height:350px;">


. Select import data:

   <img src="https://github.com/JoseCervantes22/CalHR-ChatBot/assets/133288667/5ab8ed3e-1fca-4da6-956d-816171aca3ca" alt="PROYECTO (4)-min" width="380" height="100">

5. 
