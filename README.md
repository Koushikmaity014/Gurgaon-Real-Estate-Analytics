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

    %% Professional Color Scheme
    style A fill:#EAF2FF,stroke:#2563EB,stroke-width:2px,color:#111827
    style B fill:#DBEAFE,stroke:#2563EB,stroke-width:2px,color:#111827
    style E fill:#EFF6FF,stroke:#2563EB,stroke-width:2px,color:#111827

    style C fill:#ECFDF5,stroke:#16A34A,stroke-width:2px,color:#111827
    style D fill:#DCFCE7,stroke:#16A34A,stroke-width:2px,color:#111827
    style F fill:#F0FDF4,stroke:#16A34A,stroke-width:2px,color:#111827

    style G fill:#FEF3C7,stroke:#D97706,stroke-width:2px,color:#111827
    style H fill:#FFFBEB,stroke:#D97706,stroke-width:2px,color:#111827

    style I fill:#F3E8FF,stroke:#9333EA,stroke-width:2px,color:#111827
    style J fill:#DCFCE7,stroke:#15803D,stroke-width:3px,color:#111827
