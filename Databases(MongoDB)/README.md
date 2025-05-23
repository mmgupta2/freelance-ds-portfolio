# MongoDB and Geospatial Querying for Media Analytics

## Overview

This project demonstrates how to use MongoDB for querying and analyzing semi-structured JSON-like data in a movie review dataset. The notebook includes practical examples of MongoDB’s aggregation pipeline, geospatial queries, and document-level operations — all done within a Python environment using `pymongo`.

## Business Relevance

MongoDB is widely used in modern backend systems due to its flexibility with unstructured or nested data formats. This project simulates real-world use cases such as:

- Querying a movie database for content recommendation
- Performing geospatial analysis on theater locations
- Indexing and retrieving media records for content management systems

These skills are valuable in domains like streaming platforms, location-based services, digital media analytics, and customer behavior modeling.

## Tools & Technologies Used

- Python, PyMongo, BSON
- MongoDB Atlas (or local)
- GeoPandas + Matplotlib for mapping
- Shapely for geospatial geometry
- MQL (Mongo Query Language) for queries

## Problem Statement

How can we use MongoDB to efficiently query a semi-structured movie dataset, and perform advanced filters and aggregations — including location-based analysis?

## Approach

1. **Data Setup**
   - Downloaded and unzipped the `sample_mflix` dataset
   - Connected to MongoDB instance using `pymongo`

2. **Querying & Filtering**
   - Retrieved documents from the `movies` and `comments` collections
   - Filtered based on genres, release year, and user ratings
   - Used aggregation pipelines to summarize results (e.g., average ratings per genre)

3. **Geospatial Querying**
   - Created a `theaters` collection with geospatial coordinates
   - Queried theaters within a certain radius using `$geoWithin` and `$near`
   - Visualized results using GeoPandas and matplotlib

## Results

- Executed meaningful content queries using MQL and Python
- Performed radius-based geospatial queries to find theaters near a target location
- Visualized theater density on a geographic map

## Future Improvements

- Integrate MongoDB Atlas and build a cloud-based visualization dashboard
- Index movie reviews and run text analysis on user sentiment
- Extend to other use cases like restaurant locators or event planners

## Contact

If you're building or querying flexible, JSON-based backends — especially for media, e-commerce, or geospatial services — feel free to reach out:

**Email**: [mmgupta2@wisc.edu](mailto:mmgupta2@wisc.edu)  
**LinkedIn**: [linkedin.com/in/mihirmgupta](https://www.linkedin.com/in/mihirmgupta/)

