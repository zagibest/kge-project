# Language Definition

In this section, we extracted entity types (etypes), data properties,
and object properties from OSM data source. We then formalized the
language of these concepts for each source by mapping them to the Global
Identifiers (GIDs) in the Universal Knowledge Core (UKC). In the UKC,
each GID corresponds to a unique definition of a concept. If the UKC
returns the GID of a concept, we link the concept with the GID, e.g.,
`bar_GID-14950`; otherwise, we assign a new GID to the concept, ranging
from NUM24-0 to NUM24-999. The producer aims to work with the concepts
from the three resources that we have already identified in the above
section. Meanwhile, the consumer aims to identify new concepts that will
be used to integrate these resources.

## Formalize Etypes with Properties from resources by Producer

Properties Property type Etypes

---

id, latitude, longitude, name, paths, start_destination, end_destination, length, start_latitude, start_longitude, end_latitude, end_longitude Data properties Destination, Route, Path

: Etypes with data properties

## Formalize Concepts:

![Formalize Concepts](images/words.png){#fig:example width="100%"}
