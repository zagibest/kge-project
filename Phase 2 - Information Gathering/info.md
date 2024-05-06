# Information Gathering

This section details the comprehensive data collection and processing
steps undertaken to gather footway-specific information for
Ulaanbaatar's streets. Utilizing Humanitarian OpenStreetMap Team (HOT)
as a primary source, we aimed to assemble a dataset that allows for the
detailed representation of pedestrian pathways within the urban fabric
of the city.

## Data and Knowledge Source

### Informal Data and Knowledge Source from Producer

Our team's area of interest is Ulaanbaatar so we engaged with HOT to
identify and extract informal data pertaining to footways in
Ulaanbaatar. Two key datasets were gathered:

- **Footways Dataset**: This dataset includes geospatial coordinates
  for footpaths and pedestrian areas. Attributes such as path width,
  surface type, and the presence of amenities like lighting and
  signage were collected.

- **Buildings Dataset**: As a complement to the footway information,
  we collected data on building outlines and types to provide context
  to the street network.

### Formal Data and knowledge Source from Consumer

Utilize the comprehensive OpenStreetMap dataset which provides detailed
information about Ulaanbaatar's urban layout. This dataset includes data
on streets, pathways, buildings, and other critical infrastructure
elements that are essential for creating a robust and navigable street
network.

## Resource Collection, Processing, and Scraping

We adopted both automated and manual approaches to collect and process
data from the identified sources:

- **HOT Footways Data**: The 'kgefootways.geojson' file, containing
  details of footpaths and pedestrian zones in Ulaanbaatar, was
  retrieved using HOT's Export Tool. Subsequent processing ensured
  that the data conformed to our ER model, ready for integration into
  our street network knowledge graph. (Table 2)

  ::: {#table:geojson_description}
  **Property** **Description**

  ***

  Type Specifies the type of GeoJSON object, indicating a single geographic feature.
  Geometry Type Describes the geometric shape, specifically a series of points forming a line, used for mapping linear features like roads or paths.
  Coordinates Provides the longitude and latitude coordinates that define the geometry of the feature.
  OSM ID The unique identifier for the feature within the OpenStreetMap database.
  OSM Type Indicates the OpenStreetMap classification, suggesting it is a linear feature within the 'ways' category.
  Layer Indicates if the feature is part of a multi-layered map. It is usually null if not applicable or unspecified.
  Surface Describes the type of surface of the footway, often left null if the information is not provided.
  Highway Used in OpenStreetMap to denote roads and paths, specifying its designated use (e.g., pedestrian).
  Bridge Specifies if the feature spans a bridge, usually null if no bridge is involved.
  Tunnel Specifies if the feature passes through a tunnel, typically null if no tunnel involvement.

  : GeoJSON Data Structure of Footway
  :::

- **HOT Buildings Data**: Alongside footway data, we extracted
  building data from the 'KGEbuildings.geojson' file. This provided us
  with comprehensive outlines and classifications of buildings, which
  were crucial for augmenting our street network with contextually
  relevant information. (Table 3)

  ::: {#table:geojson_building_description}
  **Property** **Description**

  ***

  Type Specifies the type of GeoJSON object, indicating a single geographic feature.
  Geometry Type Describes the geometric shape, in this case \"Point,\" representing a specific location defined by a single coordinate pair.
  Coordinates Provides the longitude and latitude coordinates that pinpoint the location of the building.
  OSM ID The unique identifier for the feature within the OpenStreetMap database.
  OSM Type Indicates the OpenStreetMap classification, \"nodes,\" suggesting it is a point feature within the map.
  Address House Number The house number of the building, often null if the information is not provided.
  Building Indicates if the feature is a building, marked as \"yes\" to denote its presence as a structure.
  Address Street The street name where the building is located, usually null if not provided.
  Name The name of the building, typically null if the building is not named or the information is not available.

  : GeoJSON Data Structure of Building
  :::

- **Data Processing and Standardization**: Both the footways and
  buildings data underwent rigorous processing. This included
  translating attributes to a standard format, reconciling
  discrepancies, and enhancing data consistency to align with our ER
  model's specifications.

- **Data Scraping and Conversion**

  - **Buildings Data**: Using Python, we extracted essential
    attributes such as coordinates (latitude and longitude), OSM ID,
    name, and type, and saved them as plain text files.

  - **Footways Data**: Similarly, Python was employed to process
    starting and ending coordinates, OSM ID, and name, which were
    then saved in text file format.

## Formal Resource Collection and Scraping from Consumer

Each file in the data abstracted from HOT represents an etype. To
systematically organize these etypes, we derived from the HOT data, as
depicted in Figure 3. This ontology, designed using the Protege tool,
includes modifications tailored to our specific research needs.

![Classes in
Protege](images/Screenshot 2024-04-16 120623.png){#fig:protege1
width="50%"}

![Property Hierarchy in
Protege](images/Screenshot 2024-04-16 120654.png){#fig:protege2
width="50%"}
