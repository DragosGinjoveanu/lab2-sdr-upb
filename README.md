# Recommendation System — World War II Aircraft (Lab 2)

## 1. Domain and Dataset Description
This project utilizes a dataset obtained from Kaggle containing technical and historical specifications for **338 military aircraft models** operated by major belligerent powers during World War II (e.g., France, Japan, USA, United Kingdom, Germany).

The dataset contains 15 total attributes (operational roles, manufacturers, crew sizes, speed, dimensions, etc.).

## 2. Registered Catalog Properties in Recombee
To define the catalog schema in Recombee via the API (using the official Python SDK), the following 9 properties were defined and submitted:

| Property Name | Recombee Data Type | Description |
| :--- | :--- | :--- |
| **PrimaryRole** | `string` | Primary operational role of the aircraft (e.g., *Medium Bomber*, *Seaplane*, *Fighter*) |
| **Manufacturer** | `string` | Manufacturing company / aircraft builder |
| **Country** | `string` | Country of origin |
| **Number** | `int` | Total number of units produced or series number |
| **ActiveSince** | `int` | Year the aircraft entered active military service |
| **LastBuilt** | `int` | Final year of production |
| **Retired** | `int` | Year the aircraft was retired from active service |
| **State** | `string` | Operational status (e.g., *Retired*) |
| **Crew** | `int` | Number of onboard crew members |

> **Note:** The unique identifier column (`Name`) is intentionally omitted from the catalog properties because Recombee natively manages item identifiers under the `itemId` key during item ingestion.
