# 📊 Data Description

## Dataset Overview
- **Source:** Maersk Turkey Transportation Management System (TMS)
- **Initial Records:** 33,794 shipment-level records
- **Final Dataset:** 22,899 valid shipments after cleaning
- **Time Period:** 12 months of historical operations
- **Geographic Scope:** 1,397 unique origin-destination pairs

## Data Structure
The optimization model expects data with the following structure:

### Required Fields
- `shipment_id`: Unique identifier for each shipment
- `movement_date`: Date and time of shipment
- `origin`: Origin city/location
- `destination`: Destination city/location  
- `container_type`: Container size (20ft, 40ft, 45ft)
- `transport_mode`: Mode of transport (road only for this model)
- `distance_km`: Distance between origin and destination
- `shipment_type`: Export, Import, or Transit

### Derived Fields (Model Creates)
- `truck_equivalent`: Container-to-truck conversion (2×20ft = 1 truck)
- `geographic_coordinates`: Lat/lon for distance calculations
- `cost_estimates`: Transportation cost calculations
- `time_windows`: Delivery constraints and schedules

## Data Privacy
Actual Maersk operational data is confidential and not included in this repository. The model code demonstrates the methodology and can be applied to similar datasets following the structure described above.

## Data Quality Standards
- **Completeness:** >95% of critical fields populated
- **Accuracy:** All shipments validated against business rules
- **Consistency:** Standardized location names and formats
- **Scope:** Road-based containerized shipments only
