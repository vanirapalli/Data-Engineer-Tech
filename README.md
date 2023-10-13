# Data Engineering Challenge Pipeline

## Overview

This pipeline is designed to address a data engineering challenge, where the objective is to fetch, process, and report on customer journey data. The pipeline involves several components and performs the following tasks:

1. Fetches customer journey data from an SQLite database.
2. Computes attribution metrics using an external API.
3. Stores the computed data in the 'attribution_customer_journey' table.
4. Generates channel reports and exports them to CSV files.
5. Handles data synchronization and transformation.

## Getting Started

### Prerequisites

Before running the pipeline, make sure you have the following prerequisites in place:

- Python 3.x
- SQLite database with a file named 'challenge.db'
- API key for accessing the attribution computation API
- Required Python libraries:

    - `requests`
    - `logging`

### Configuration

1. Open `main.py` and update the following configuration parameters:

    - `api_key`: Replace with your API key.
    - `start_date` and `end_date`: Specify the desired time range for data fetching (optional).

## Usage

To run the pipeline, execute `main.py`:

```bash
python main.py --api_key YOUR_API_KEY --start_date YYYY-MM-DD --end_date YYYY-MM-DD
