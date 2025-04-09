# Natural Language Data Understanding with Azure OpenAI, LangChain, and Azure Databricks

## Project Overview

This project demonstrates how Azure OpenAI, LangChain, and Azure Databricks (with Unity Catalog) can be integrated to facilitate natural language understanding of datasets. By leveraging randomly chosen datasets from [data.gov](https://data.gov), we aim to enable users to explore and comprehend their data intuitively through natural language queries. The goal is to highlight how Azure OpenAI can assist in understanding datasets while also enhancing domain knowledge.

## Features

- **Azure OpenAI Integration**: Uses Azure OpenAI (via its Python package) to analyze data and provide natural language insights.
- **LangChain for Language Models**: Integrates LangChain to streamline interactions with language models and enhance contextual understanding.
- **Azure Databricks**: Employs Azure Databricks for scalable data processing and analysis, utilizing Unity Catalog for data governance and organization.
- **Random Dataset Selection**: Pulls datasets from data.gov to showcase how the solution adapts to various types of data.
- **Natural Language Interface**: Allows users to explore and query their data in a conversational, natural language format.

## Architecture

1. **Dataset Preparation**:
   - Randomly selected datasets are downloaded from data.gov.
   - The datasets are ingested into Azure Databricks and cataloged using Unity Catalog.

2. **Data Processing**:
   - Azure Databricks preprocesses and organizes the datasets.
   - Rows from the processed tables are prepared for analysis.

3. **Azure OpenAI Analysis**:
   - The datasets are passed to Azure OpenAI via its Python SDK.
   - Azure OpenAI analyzes the data, providing natural language summaries and insights.

4. **LangChain Integration**:
   - LangChain facilitates the orchestration of natural language queries.
   - Users can interact with the data through a conversational interface.

## Installation

To replicate this project, follow the steps below:

### Prerequisites
1. Azure Subscription with access to:
   - Azure Databricks
   - Azure OpenAI Service
2. Databricks CLI installed and configured.
3. Python environment with the following packages:
   - `azure-ai` (Azure OpenAI SDK)
   - `langchain`
   - `pandas`
   - `requests`
4. Terraform (optional, for provisioning Azure resources).

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/natural-language-data-understanding.git
   cd natural-language-data-understanding
