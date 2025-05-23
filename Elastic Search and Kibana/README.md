# Interactive Data Search & Mapping with Elasticsearch and Kibana

## Overview

This project demonstrates how to use Elasticsearch for indexing and querying structured JSON data, and Kibana for building interactive visual dashboards — including geographic map visualizations. It simulates how a team might load business data, perform advanced queries, and visualize real-time metrics or locations.

## Business Relevance

Elasticsearch is widely used in:
- Log and event monitoring (e.g., ELK stack for DevOps)
- Full-text search engines
- Location-based analytics
- Business dashboards for real-time KPIs

Kibana allows teams to build **interactive visualizations** and **geo maps** without needing complex frontend code. This project mimics a use case where a city or business wants to explore events or infrastructure data on a map.

## Tools & Technologies Used

- Elasticsearch (local instance or Elastic Cloud)
- Kibana (dashboard interface)
- Python (`elasticsearch` library) for indexing
- GeoJSON for coordinate encoding
- JSON, REST API interaction

## Problem Statement

How can we build a real-time searchable data layer that:
- Ingests JSON documents (like events, inspections, or facilities)
- Allows fast, filtered queries by location or category
- Supports visual analysis with maps and time series dashboards

## Approach

1. **Elasticsearch Setup**
   - Connected to a local Elasticsearch instance with secure login
   - Created custom indices using mappings for nested and geo fields

2. **Data Ingestion**
   - Loaded multiple JSON datasets using bulk indexing (via Python and REST)
   - Included geospatial fields for location-based search and mapping

3. **Search & Querying**
   - Built compound queries using Elasticsearch DSL
   - Tested filters by keywords, ranges, and location bounding boxes

4. **Visualization with Kibana**
   - Created dynamic dashboards with pie charts and data tables
   - Built a live geospatial map of indexed data using Kibana's Maps UI

## Results

- Successfully indexed thousands of structured JSON records
- Enabled high-speed keyword and geospatial queries through Python and Kibana
- Built interactive dashboards showing distribution, location, and volume of key metrics

## Future Improvements

- Connect Kibana to live data streams for real-time updates
- Use Logstash for automated log ingestion and preprocessing
- Extend to alerting or anomaly detection using Kibana's rule engine

## Contact

If you're interested in building interactive data dashboards, log monitoring pipelines, or scalable search interfaces using Elasticsearch, feel free to reach out:

**Email**: [mmgupta2@wisc.edu](mailto:mmgupta2@wisc.edu)  
**LinkedIn**: [linkedin.com/in/mihirmgupta](https://www.linkedin.com/in/mihirmgupta/)

