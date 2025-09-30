# OLAP  
*A lightweight project for exploring OLAP (Online Analytical Processing) concepts, with a focus on data modeling*  

VICTOR KIPNGENO ROTICH 388

## Table of Contents  
1. [Overview](#overview)  
2. [Features](#features)  
3. [Architecture & Design](#architecture--design)  
4. [Getting Started](#getting-started)  
   - [Prerequisites](#prerequisites)  
   - [Installation](#installation)  
   - [Usage / Running the project](#usage--running-the-project)  
5. [Project Structure](#project-structure)  
6. [Examples / Sample Data](#examples--sample-data)  
7. [Contributing](#contributing)  
8. [License](#license)  
9. [Contact / Acknowledgements](#contact--acknowledgements)  

---

## Overview  
The OLAP project is a lightweight experimental / educational tool intended to help explore OLAP concepts, particularly around **data modeling**.  
It is designed for:  

- Learning how dimensions, hierarchies, fact tables, and measures tie together  
- Prototyping or experimenting with small datasets  
- Demonstrating mapping of analytical queries to underlying relational tables  

---

## Features  

- Representation of fact tables and dimension tables  
- Support for hierarchical dimensions (e.g. Year → Quarter → Month)  
- Aggregation of measures (sum, count, etc.)  
- Query planning / translation (OLAP queries → relational operations)  
- Lightweight and minimal dependencies  

**Planned Features:**  
- Roll-up and drill-down operations  
- More complex measures (ratios, calculated fields)  
- Performance optimization with caching  

---

## Architecture & Design  

- **Data Model Layer** – defines fact and dimension schemas  
- **Query Layer** – accepts OLAP-style queries and maps them to SQL / relational operators  
- **Storage Layer** – handles data access (CSV, database, or in-memory tables)  
- **Aggregation Engine** – computes aggregated results  

---

## Getting Started  

### Prerequisites  
- Python 3.8+  
- Recommended: virtual environment  

### Installation  

```bash
git clone https://github.com/VICTOR21-A/OLAP.git
cd OLAP

# Create a virtual environment (optional)
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

# Install dependencies
pip install -r requirements.txt

