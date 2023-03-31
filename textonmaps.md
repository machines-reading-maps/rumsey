---
layout: default
title: What is Text on Maps?
nav_order: 2
---

# What is Text on Maps?

About 57,000 of the georeferenced maps from the collection have been processed with a machine learning tool called mapKurator to collect all the **text on maps**, i.e. every piece of text (printed or handwritten) that appears on a map, including place names, but also information like a map’s title or its scale, or the names of the people involved in producing the map. Through this process of **automatic annotation**, this approach turns the text on maps into structured data (text on maps data): the enormous amount of data that has been collected from these maps is now searchable. 

You can now search this part of the collection for any place or word appearing anywhere on the maps, no matter how small or obscure. 

## Why is this different?

Usually, when you search a catalogue of digitised maps, the words that you provide the search engine are matched against **metadata** stored in a record about each document. This usually includes essential information documented by librarians or archivists such as a title, the creator’s name, the publication details, the size of the media, brief description, and other fields. 

Metadata are, in a way, the digital heirs of the information that has been written on library cards or in collection inventories for centuries. They are therefore a vital component of any digital library or archive. It is thanks to metadata that we are able to find anything. However, given the history of using record metadata to capture information about an item rather than its content, it’s not logistically possible for metadata to store the information about every single place mentioned in each map. This is the reason why, if you look for a place in a map collection, you can only find maps that have that name appearing in their metadata.

Making it possible to search about ½ of the David Rumsey Map Collection (as of 2022) based on the content of a map rather than only its metadata is a major shift in the history of searching cartographic collections. 

While library patrons have become used to searching books via their content as well as their titles and authors, such technology has not yet been applied to visual media like maps. Exposing text on maps alongside traditional catalog record metadata transforms how people search maps and why people might be interested in historical maps altogether: now the content of large sets of maps can be examined as data that tells us not only about the history or cultural context of specific places, or of regional mapping traditions, but also about broader social and cultural developments. 

## How do you identify map text at scale?

To learn more about the methods used here, check out the Github repositories for 
1) the [mapKurator]([url](https://knowledge-computing.github.io/mapkurator-doc/#/)) tool for generating map text data, and 
2) the [annotation interface]([url](https://github.com/machines-reading-maps/luna-annotorious-client)) embedded within the website. 

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

