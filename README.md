## 🛠️ Data Preprocessing

The raw 99acres property listings were cleaned, standardized, and transformed into a structured Gurgaon real-estate dataset.

### Processing Workflow

```mermaid
flowchart TD
    A["Raw Flats Data<br/>flats-flats.csv"] --> B["Flats Preprocessing"]
    C["Raw House Data<br/>independent-house.csv"] --> D["House Preprocessing"]

    B --> E["flats_cleaned.csv"]
    D --> F["house_cleaned.csv"]

    E --> G["Merge Datasets"]
    F --> G

    G --> H["gurgaon_properties.csv"]

    H --> I["Level-2 Processing<br/>Create Sector + Feature Pruning"]

    I --> J["gurgaon_properties_cleaned_v1.csv"]
