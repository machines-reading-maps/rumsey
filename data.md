---
layout: default
title: Understand and Access the Underlying Data
nav_order: 3
---

# Understand and Access the Underlying Data

The David Rumsey website indexes output from mapKurator in ordert to make text on maps searchable. Below you can see how the data fields from the mapKurator output file (a geojson) map onto the indexed fields in the “Text on Maps” search in the website.

##### Indexed Fields
- “Mapkurator output” - mapKurator's predicted transcription of text within its predicted bounding polygon
- “MapKurator output (post-processed)” - output from mapKurator's PostOCR module which updates text content based on a fuzzy string match to a dictionary of OpenStreetMap feature names (content in this field is always CAPITALIZED).
- “User annotations” - updates to mapKurator predictions by users like you
- “All Text on Maps” - combination of all of the above

##### mapKurator Data Fields Mapped to DavidRumsey.com “Text on Maps” Search
- `text` mapped to “Mapkurator output”
- `postocr_label` mapped to “MapKurator output (post-processed)”

In the basic search, users will see results from the “MapKurator output (post-processed)” field. In advanced search, you can select which indexed field(s) you wish to query.

Snapshots of changes to the dataset based on user annotations will include a new field containing those annotations. This annotation will be associated with a user name (that defines a contribution from a human as opposed to a machine-inferred annotation) and time stamp. Users who save changes to the data produce the following update:

```
const changedTranscription = {
type: 'TextualBody',
purpose: 'transcribing',
value: '<transcription>',
creator: {
type: 'Person',
name: '<username>'
},
created: <iso timestamp>
};
```



## Access the data

If you are interested in working with this data using your own computational methods, you can access Version 1 (V1) of the full, **open access dataset** alongside its documentation. (Link to be provided shortly.)

Please note that this machine-generated (inferred) data has not been evaluated, validated, or otherwise improved. It therefore **contains many errors** which will vary significantly depending on many factors. 

There are multiple versions of the data. V2 and V3 will be made available as open datasets soon and links will be provided here. 

On davidrumsey.com, you are searching V2 of the data (as of April 2023).
