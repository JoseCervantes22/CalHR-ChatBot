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

Introduction
Benie the Bot is a virtual assistant built to streamline and simplify the process of accessing and understanding employee benefits information within the CalHR organization. It leverages multiple technologies to provide quick and accurate responses to common benefits-related questions and guide employees through various benefit-related processes.

Architecture
![Architecture](https://github.com/JoseCervantes22/CalHR-ChatBot/assets/133288667/beb83862-8278-450f-8fba-c5e1cbac3ac6)

Components
Power Apps Package: This package includes a Power Virtual Agents (PVA) chatbot and a Power Automate API that connects to Azure OpenAI. It allows Benie to interact with users and retrieve responses from the ChatGPT model.

OpenAI ChatGPT Deployment Configuration: This repository includes the configuration files and scripts required to deploy and manage the ChatGPT model from OpenAI, enabling natural language understanding and conversation with users.

Cognitive Search: Instructions and resources are provided to set up Cognitive Search, allowing you to index and search the PDF documents provided by CalHR. This feature enhances the bot's ability to retrieve relevant benefits information.

Features
PDF Document Integration: Benie v0.3 utilizes the PDF documents provided by CalHR as the primary source of information, making it a comprehensive resource for benefits-related inquiries.

Powerful Search Capability: With Cognitive Search integration, users can search and access specific information from PDF documents quickly.

Chat-Based Interaction: Benie provides a conversational interface for users to ask questions and receive benefits-related information in a natural and user-friendly manner.

Modular Architecture: The components are designed to be modular, making it easier to update and expand Benie's capabilities.

Upcoming Features: Web crawling and web scraping capabilities are scheduled for Benie v0.4, allowing Benie to gather information from online sources and further enrich its knowledge base.

Installation
To get started with Benie the Bot and its components, please refer to the individual installation guides and setup instructions provided in their respective directories.

Documentation
For detailed information on how to use and configure Benie the Bot and its components, please refer to our documentation:

Power Apps Package Documentation: Instructions for setting up the Power Apps package and integrating it with the chatbot.

OpenAI ChatGPT Deployment Guide: Guidance on deploying and managing the ChatGPT model from OpenAI.

Cognitive Search Setup Instructions: Steps to set up Cognitive Search for indexing and searching PDF documents.

Contributing
We welcome contributions from the community to enhance and improve Benie the Bot. If you would like to contribute, please review our Contributing Guidelines.

License
TBD.
