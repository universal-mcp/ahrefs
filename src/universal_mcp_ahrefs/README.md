
# Universal Mcp Ahrefs MCP Server

An MCP Server for the Universal Mcp Ahrefs API.

## 📋 Prerequisites

Before you begin, ensure you have met the following requirements:
* Python 3.11+ (Recommended)
* [uv](https://github.com/astral-sh/uv) installed globally (`pip install uv`)

## 🛠️ Setup Instructions

Follow these steps to get the development environment up and running:

### 1. Sync Project Dependencies
Navigate to the project root directory (where `pyproject.toml` is located).
```bash
uv sync
```
This command uses `uv` to install all dependencies listed in `pyproject.toml` into a virtual environment (`.venv`) located in the project root.

### 2. Activate the Virtual Environment
Activating the virtual environment ensures that you are using the project's specific dependencies and Python interpreter.
- On **Linux/macOS**:
```bash
source .venv/bin/activate
```
- On **Windows**:
```bash
.venv\\Scripts\\activate
```

### 3. Start the MCP Inspector
Use the MCP CLI to start the application in development mode.
```bash
mcp dev src/universal_mcp_ahrefs/mcp.py
```
The MCP inspector should now be running. Check the console output for the exact address and port.

## 🔌 Supported Integrations

- AgentR
- API Key (Coming Soon)
- OAuth (Coming Soon)

## 🛠️ Tool List

This is automatically generated from OpenAPI schema for the Universal Mcp Ahrefs API.


| Tool | Description |
|------|-------------|
| `crawler_ips` | Retrieve the list of public crawler IP addresses from the API. |
| `crawler_ip_ranges` | Fetches the current public crawler IP ranges from the API, optionally specifying output format. |
| `limits_and_usage` | Retrieves current API subscription limits and usage statistics from the service. |
| `batch_analysis` | Submits a batch analysis request with specified parameters and returns the analysis results as a dictionary. |
| `serp_overview` | Retrieves a SERP (Search Engine Results Page) overview report based on specified selection, country, and keyword criteria. |
| `overview` | Retrieves rank tracking overview data for a specified project, date, and device. |
| `competitors_overview` | Retrieves an overview of competitor rankings for a specified project and criteria. |
| `projects` | Retrieves a list of site audit projects from the configured base URL, optionally specifying an output format. |
| `domain_rating` | Fetches the domain rating and related metrics for a specified target and date. |
| `backlinks_stats` | Retrieves backlink statistics for a specified target and date, with optional filters for protocol, mode, and output format. |
| `outlinks_stats` | Retrieves outbound link statistics for the specified target from the site explorer API. |
| `metrics` | Retrieves metrics data from the site explorer API endpoint. |
| `refdomains_history` | Retrieves the historical data of reference domains from a specified site. |
| `domain_rating_history` | Retrieves historical domain rating data for a specified target within a given date range. |
| `url_rating_history` | Retrieves URL rating history data for a specified target within a date range. |
| `pages_history` | Retrieves historical page data for a target using specified filters. |
| `metrics_history` | Retrieves historical metrics based on specified parameters. |
| `keywords_history` | Fetches the historical keyword rankings and performance data for a specified target within an optional date range and set of filters. |
| `metrics_by_country` | Fetches site metrics grouped by country for a specified target and date. |
| `pages_by_traffic` | Retrieves a list of top pages for a specified target domain or URL, ranked by estimated organic search traffic. |
| `all_backlinks` | Retrieves all backlinks information for a specified target using various query parameters. |
| `broken_backlinks` | Fetches broken backlink data for the specified target from the site explorer API endpoint. |
| `refdomains` | Retrieves referring domains data for a specified target using the Site Explorer API endpoint. |
| `anchors` | Fetches anchor text distribution data for a specified target using given query parameters. |
| `linkeddomains` | Retrieves linked domains for a specified target using the site explorer API endpoint. |
| `linked_anchors_external` | Fetch linked external anchor data for a specified target using provided selection and filtering criteria. |
| `linked_anchors_internal` | Fetches internal linked anchor data for a specified target from the site explorer API, applying optional filtering and query parameters. |
| `organic_keywords` | Retrieve organic keyword data for a specified target and date from the Site Explorer API endpoint. |
| `organic_competitors` | Retrieves organic competitors data for a specified target using the Site Explorer API. |
| `top_pages` | Retrieves top pages data for a specified target and date from the site explorer API with customizable query parameters. |
| `paid_pages` | Fetches paid pages data from the Site Explorer API based on specified filters. |
| `best_by_external_links` | Fetches data about the best-performing pages of a target site based on external links, with various filtering and output options. |
| `best_by_internal_links` | Retrieves the best-performing internal links for a specified target using the site explorer API endpoint. |
| `total_search_volume_history` | Fetches the total historical search volume data for a specified target within a given date range and optional filters. |
| `keyword_explorer_overview` | Retrieves an overview of keyword metrics and data from the keywords explorer API endpoint based on the specified filters and parameters. |
| `volume_history` | Fetches the historical search volume for a given keyword in a specified country. |
| `volume_by_country` | Retrieves search volume by country for a given keyword. |
| `matching_terms` | Retrieves matching keyword terms from the keywords explorer API based on specified filters and search parameters. |
| `related_terms` | Retrieves related keyword terms for a given selection and country, with optional filtering and pagination. |
| `search_suggestions` | Fetches keyword search suggestions from the keywords explorer API based on the provided filtering and query parameters. |

## 📁 Project Structure

The generated project has a standard layout:
```
.
├── src/                  # Source code directory
│   └── universal_mcp_ahrefs/
│       ├── __init__.py
│       └── mcp.py        # Server is launched here
│       └── app.py        # Application tools are defined here
├── tests/                # Directory for project tests
├── .env                  # Environment variables (for local development)
├── pyproject.toml        # Project dependencies managed by uv
├── README.md             # This file
```

## 📝 License

This project is licensed under the MIT License.

---

_This project was generated using **MCP CLI** — Happy coding! 🚀_
