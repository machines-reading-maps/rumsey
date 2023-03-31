---
title: Home
layout: default
nav_order: 1
description: "Guide to Searching and Annotating Text on Maps"
permalink: /
---


# Guide to Searching and Annotating Text on Maps
{: .no_toc }

- Learn about new and experimental features that have been introduced to a subset of maps in the David Rumsey Map Collection. 
- Discover what’s new, how to make the most of the new available tools, and how new computational methods enabled this new way search maps. 
- Find out how to get involved.


## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}



## Quick Start

### Search Text on Maps

In addition to a traditional search of Catalog Data (e.g. titles, authors, dates), the Luna Viewer now allows you to search the text content of many maps. We call this ‘Text on Maps”. 

Only maps that have been geo-referenced can be searched by the text they contain.

Using the Advanced Search, you can perform combined searches of Catalog Data and Text on Maps. In the Advanced Search, you also can specify which version of the Text on Maps you want to search. Read more about these options **here**.  




### View Text on Maps

Not only can you view the text you searched for, you can also view all other text on this map and correct the underlying data!


When you arrive from the search page, you will see only your search term highlighted. To see or hide all Text on Maps for this map, click on the icon you see below in the top left corner of the map image.
<img width="42" alt="Screen Shot 2023-03-16 at 17 06 24" src="https://user-images.githubusercontent.com/20363927/225681301-0f4aadf6-9179-4c08-b948-a70eeb49de30.png">


### Become a Contributor

To edit a particular selection, click on the highlighted text. Now, you will see the annotation pop up. To learn more about how to annotate (correct, confirm, etc.) text on maps, read this guidance.


To edit an incorrect bounding polygon around text, click on the highlighted text. In the pop up, click ‘edit’. You will see the vertices of the polygon appear: you can move these to improve the way that the polygon surrounds the text, or you can delete a polygon that has been created in error. Read this guidance for more details.


***Please note, you must be logged in to edit the data.***


## Search Text on Maps

If you want to try this new feature, type a word or phrase that interests you in the search field in the top left of your browser window. Then, from the drop down menu, select “Text on Maps”. 

*The other options (“Catalog Data”, “Catalog Data & Text in documents”, and Advanced Search) are reviewed in more detail below.*

#### Search Tips

- The initial prompt for searching “Text on Maps” accepts 1-word queries. If you want to search for multiple words, please see the section on this below. 
- Searches are not case sensitive, nor can they accept regex.
- Although we are working on improving the performance of mapKurator for all languages, it is currently not possible to search Text on Maps for words in non-latin alphabets.
- Your search results will be displayed in a random order that will change each time. So, if you run the same search more than once you will see the same results, but displayed in a different order. 
- If you want to refine the results of your query with filters based on Catalog Data, you need to use the Advanced Search feature.

When you select “Text on Maps”, you will search for occurrences of the word on the entire dataset. (Read more here to learn about how this data was created.) For example, if you type “Paris” you will see how many times that word is printed on any of the ~57,000 maps in the collection that we have processed. (This includes text within and outside of the neatline, e.g. it includes map titles and other descriptive information.) The searchable datasets represents content on David Rumsey collection maps that have been digitized and georeferenced up to 2022. 

*Note: [Georeferencing](https://en.wikipedia.org/wiki/Georeferencing) means establishing points on the scanned image that point to locations on the earth. These control points allow content on the digitized map to be geolocated. [You can try georeferencing out yourself.](https://www.davidrumsey.com/view/georeferencer)*

### Searching for Multiple Words
mapKurator output is saved only as individual words: there is no prediction of phrases, for example, for places names that contain more than one word (e.g. “South Ponte Vedra Beach”)

However, multi-word search is possible because of the way the data has been indexed. Briefly, multi-word searches will be successful when adjacent words are within a 2-character length from the two points of the bounding polygon that are the furthest away from each other. This is based based on the size of the characters in the least common word in the search, e.g. “Ponte” below.

![2oL2F3hBMLrYUlWA0Vef-XW-jS26IRqNm-sUsxJs95Zgx8jxw30upNdQ0AIHFUGeqisVZU7WYovVyAjZEyRiHKE89_rjZ8DDFxzL78Cj0IXSUM0U695o5peja7MM](https://user-images.githubusercontent.com/20363927/229169937-1a136dbd-8804-4cc3-b696-1359a32fbfd2.png)

![02DmRWhg_e6pFx_V6-t2sADuJmMzLqFJXWE_8VqlwXOp_Y1ShNwhG9_R6sBi9zL4wPbmHOXhCVEL_QKWgW9Li-NNAf-7NlB2PVwhRDy-mmItjGQX86lgBtEtWaf3](https://user-images.githubusercontent.com/20363927/229170004-34e034d7-c92c-4058-be5e-2827dc238769.png)
Example of multi-word search.



### Advanced Search
Advanced searching allows you to combine queries of Text on Maps with Catalog Data, i.e. you can leverage the power of the search by text, but also filter the results by their metadata. You can access the advanced search options by clicking on the dropdown menu in the search field.
 
![PbCLKmhsHkzRQ-Xe6I8cJxD4Rnk9QvaG2S3qO11xfyBsBx75X5byZ2h2KpNwfgw5JZ-3Fsg95fUVGyJTW_SRU6h7tda2YEpu03p__dNnCASfhSWeiCXQ0kTxtunZ](https://user-images.githubusercontent.com/20363927/229170122-84af1413-ff76-4792-8289-f4783d631481.jpg)

Clicking on the “Advanced Search” option, you will access a dedicated interface where you can refine your queries in the collection, using the different fields. You can choose one or more criteria in your search. 

![Yd9CvV-fO12m40q9mPxNn2HMFPH3C9-K_UsoTWBiNnv7N3v-UtZ4t-nPWmV_Xp2y50HZDlkK21hewHvSZ1PwbAq4lW1JJRg1vZMit1xZZWhag45CsseiU3mwfTNz](https://user-images.githubusercontent.com/20363927/229170197-6ebcf4e3-5e92-4083-b54b-860d43441a52.jpg)


1. **Find all these words**: Click on the drop down menu of the first white box and select one of the data fields from the David Rumsey Map Collection catalog, for example “country”. In the corresponding box on the right, you can type the value that you want to match, for example “United States”. As a result, you will get all maps that have both the words “United” and “States” as a value for “country”.

2. **Find any of these words:** Click on the drop down menu of the first white box and select one of the data fields from the David Rumsey Map Collection catalog, for example “country”. In the corresponding box on the right, you can type the value that you want to match, for example “United States”. As a result, you will get all maps that have the words “United” OR the word “States” as a value for “country”. (this will include, for example, maps featuring the United Republic of Congo).

3. **Find this exact wording:** Click on the drop down menu of the first white box and select one of the data fields from the David Rumsey Map Collection catalog, for example “country”. In the corresponding box on the right, you can type the value that you want to match, for example “United States of America”. As a result, you will get ONLY the maps that exactly match your query and have “United States of America” as a value (this will NOT include maps that have only “United States” as a value).

4. **Date range:** Click on the drop down menu to select the data field you want to search. The options are either “date” (the date the map was printed) or “pub date” (the publication date of the item in which a map appears, for example an atlas). In the corresponding fields on the right, enter two dates that represent the beginning and end of your date range. For example “1830” and “1850”. As a result, you will see all the maps that have a date (or pub date depending on your query) that falls in that range. You can combine this filter with the previous one.

5. **Words in text on maps:** click on the drop down menu to choose what type of text on maps you want to search. 

The options are:
- “Mapkurator output”: This is the raw output of the machine learning pipeline (mapKurator) applied to the maps, in other words it is the corpus of mapKurator's predicted transcription of text within its predicted bounding polygon. No subsequent edits or processes have been applied.
- “MapKurator output (post-processed)”: In this dataset, the output from mapKurator has undergone another processing step. Based on the predicted transcription and the geographic coordinates associated with it, another machine learning module attempts to match the predicted text against a vocabulary of feature names in Open Street Map. Content in this field is always CAPITALIZED. This process may help reduce errors, but can also introduce new ones, and it could make some less known features less visible.
- “User annotations”: Updates to mapKurator predictions created by users like you, through edits and/or validation of automatic transcription generated by mapKurator. Currently, this dataset is very small but it will grow with time. The index of annotations is updated daily, so new annotations may not be immediately searchable.
- “All Text on Maps”: includes all of the above.

Then, in the field on the right, write the word you want to search in any of the selected options for Text on Maps.

![ZbXUeWkqUXyGdwzNEUIuhaK1IBRLFedB-aic7-hDw5IIGWL7sOf5e71c1He4TO9xKLPOqo8AK7xHz-F0H8dghTXFF8vkjGhRXUdOx5Sy4GQG9SUERtL6wxtj3jZb](https://user-images.githubusercontent.com/20363927/229170281-c30157a9-a462-4fbd-a700-85882f78ba2c.jpg)



*Please note: In the regular, non advanced search, the “Text on Maps” searches the “MapKurator output (post-processed)” data by default.*

*Please also note: once you refine the search in this way, it’s not possible to further organize the results. To complete searches with more complex sorting and filtering, please use the “Catalog Data” search without also including the “Text on Maps” option.*

##### Here are some examples:
1. You can refine the search to produce results only for maps that were published between 1700-1800 and where the sheet contains the raw mapKurator output for “Paris”. In the search box in the browser this is expressed as: pub_date=1700...1800 AND ocrText="Paris" LIMIT:RUMSEY~8~1. `Pub_date` represents the date range and `ocrText` represents the raw mapKurator output.
2. A variation on this search limits by publication date, but searches the post-processed mapKurator transcriptions instead of the raw mapKurator output: pub_date=1500...1700 AND postOcrText="France" LIMIT:RUMSEY~8~1

![95_S84Xk9EMk4tx07IMzXt_3k5904m04jPy1TbgLxa1Q_d3vtri3nF553ukKGd0HW4aZIg2q3RWMaPsABz8-nPZIoxPxxSa1wwXDlVpJ0AttUBFt6Zgok1zAHev_](https://user-images.githubusercontent.com/20363927/229170356-8b6b6f86-25f9-48e7-9ee1-d71da57cf730.png)


Happy exploring!

## View Search Results

### Masonry View
<img width="103" alt="vDcsdOla8jQVeNAgDY9VZM9_KmFGwAUqWBjRX8p2OXNlNxTvLk1BvGml4kQFODyJScnsoUpi_vbdynRVRV52k03Wumfs7po1_jpIbGtm1u8w0btnCvDIzQttv-VC" src="https://user-images.githubusercontent.com/20363927/229170528-577b7510-0aff-4129-b796-2ffe8817a1c1.png">


By default, you will be viewing the results of your Text on Maps search in “masonry view”, i.e., a collage of all the map text that matches your search. 

If you hover the pointer over any result’s “brick”, you will see a small preview of the entire map and a yellow pin signaling the position of that particular annotation in relation to the map. 

The masonry view is a quick way to compare the variety of ways that a word or words appears on maps from many cultures and centuries. 

It’s also a handy way to visualize errors in the automatic text detection and recognition parts of the method creating this data. To learn more about this, you can read more **here**.

![d31Y41N0zcKdjvf9M2xap4EiqXthtAobPYwzR_U3MoCkbQoGVjPWLILA4qRR0yUZYX_QeC1-KeajrkMzYRx1m42aqj9CR4sEc5Vb7d4cB4LtMBze-1-FtGVAWRfg](https://user-images.githubusercontent.com/20363927/229170594-4cd434e9-87e2-4f0a-bbe9-77223d8839da.png)




Tile View
<img width="97" alt="zSxgKYHyDBsKf_UQOtK21gojPt0NH2C7O-W55z9w8SOwwJlHh06H5X4KvbCCGqpRa6aznCVpT-4XiBoTXHc9c0QWdzbKGMsm7BoI5fGvk6Bu7Dya5QaBRzKa3ozD" src="https://user-images.githubusercontent.com/20363927/229170677-1fd71a78-abab-40a5-87b1-7b961627e4a6.png">

You can also select the “tile view”, to directly see all thumbnails of the maps that match your search. This view is more like the traditional view you see when searching via Catalog Data (e.g. the title).

In both the masonry or tile views, if you click on any of the map thumbnails, you will be taken to a larger view of the map. Here you can also see all the machine-generated bounding boxes around the labels and their transcriptions by clicking the lines icon in the toolbar (see annotating Text on Maps).


## Become a Contributor

When you look at the machine-generated annotations (“MapKurator output” or “MapKurator output (post-processed)”), you may notice errors. 

Maps, and the historical ones in particular, are a very challenging input data source for text detection and  recognition (or, “text spotting”, as used by mapKurator), and the quality of the results will vary depending on the color(s) of the background, the fonts, the printing technique, the language, the conservation status, and so on. 

**We invite all the users of the David Rumsey Map Collection to team up with the machine and improve or confirm the annotations.** 

If you spot a mistake, please consider contributing a better transcription, and/or a more accurate bounding box. 

### Text transcription
You can fix a text label’s transcription so that it matches what appears on the sheet. 

Please note: The goal is to **exactly replicate what is on the map**. 

This includes what might be perceived as “errors” given changes to place names or other factors. Here are some guidelines to help you:

- If there is a typo on the map, or a place name has changed (based on your knowledge), or you want to write the place name in a different language (transliteration), **do not make changes that do not reflect what is on the map**. 
- Similarly, **do not expand abbreviations**. 
- Please **include punctuation or spaces** as relevant.

If you are interested in learning more about best practices in annotating text on maps, the annotation guidelines developed by Machines Reading Maps can be found [here](https://github.com/machines-reading-maps/Tutorials-Newsletters/wiki/Map-Text-Annotation-Guidelines). 

Editing is very easy! 
1. Click on the annotation you want to improve. You can view previous transcriptions by unfolding the “n more transcriptions” part of the box. 
2. Click on “Edit” to add a transcription that will be saved under your user name.
3. The bounding polygon and the text field will now be editable and you can change the text transcription as needed.
4. It is possible to cancel your changes or to save them by clicking on the relevant buttons.
5. Afterwards, your transcription will be immediately visible (they will be searchable after 1 day).


##### Visual examples of editing: 
<img width="543" alt="1Hc2YdBygHaDKoQW0ql0jenhG9y2OTLo-oJzF6B_Z5-B80ZimcV5UevXBHaF0fZVjvzRab0jA_3BcvrdFl6rxOTEOTm0BSJW4mlKkKpUsBBU1gX3K7LpoXXI0SyN" src="https://user-images.githubusercontent.com/20363927/229171274-f6ee283c-bedd-4f00-9732-6678adfaecf7.png">

<img width="519" alt="0r6bH6HRhVcYtFRCg9zHB3NUWtEQUXA3v7i0wpeAES6e-7koreFPkgMdhOpdorln4_3L786671q4-8fdor8K5_dffudsIOP3FXjeDCerwWZA3t41RPBnCra9q6S3" src="https://user-images.githubusercontent.com/20363927/229171349-3245f2e7-d6c9-487e-973d-45c18868ffc6.png">

<img width="509" alt="_ngE_IeLMdybIWa2uKV_U9o4CJmTH5IMvK0L8n0MUyvwU4xDau92VODhWAm9Ysr9X4_C87GZKVjgGTEFzoP1Q3jmkxD4KJbm8ZKecfd67RcXlwpzJUCVCSxSaX8w" src="https://user-images.githubusercontent.com/20363927/229171382-f7340bff-ff30-4764-994f-7e2fe8737c85.png">

<img width="364" alt="gxepJLBgy3Qk-6TIqbq7sIwAr9Xu86pU7_2bAX_n5jWzN0Z8jYUCA_NWGkt7KTnWquwxa9Owghqg-ptvLh7tLyyh3JfJcVAK3FUS_ja_xm0ZGgTR0n_EnbLSbXog" src="https://user-images.githubusercontent.com/20363927/229171423-463987c9-86fc-4868-8b58-0ed5f9787a40.png">




### Bounding polygons
When you select an annotation, several points along the polygon become active, and you’ll be allowed to move them around, changing the shape of the polygon. However, you are not currently able to draw new polygons around text. 

If the polygon incorrectly surrounds a word, you can modify the polygon around that text.

Bounding polygons may be incorrect when:
- They do not include all the characters of one word
- Two polygons overlap/duplicate the transcription of a single word
- Fail to capture a text label at all

##### Visual examples of these cases:

<img width="737" alt="x1J_3tWjVKwAWoHqYt9AEtUHuAQ-YzjME_As1HmTJS4v3GQvs8LsU6X7SWkjWKSKSUFb5tA6FDeTNVnipUdvSEc6Wu5kHM2azNU0rrXIbC1_XYilVcDZq2uQKTQU" src="https://user-images.githubusercontent.com/20363927/229173664-bad9dd91-9027-4b2a-8ae5-f1206cdde50a.png">

<img width="296" alt="qdU6K1fb4xx4oqP-vz_QBE63rSQonfFC3MGLomVLIAIRSTlMx5jYX5fxs28GA8YmlQIsDZyhaOyhyk4QjqOk4wr-vA0fsaohKE_n2yuelO-sWhv7cVWiZ6y_gtKB" src="https://user-images.githubusercontent.com/20363927/229173717-5ea65192-9832-4998-adf2-358a680014a3.png">

### What happens to my annotations?
Annotations are stored and will appear to the public online immediately, however changes will be searchable only after a delay of 1 day. These changes are logged alongside the existing data: nothing is removed from the underlying data.  

Your changes will be identified by your user name. 

Once the text and the bounding polygon have been confirmed by 1 user, a green check will appear next to the transcription. This operates as a guide to future users so that they can focus elsewhere.

<img width="398" alt="Ks8mz4y97nrwRuBLQvsnaL5pSNr5_DVpQv-ij4QoExg5t1_Z7WVsO12shMTS2yrChhHCSRNq6pio85am8rWHkB_mBlIMFaQ2KsSJDRky8BHjkn4ClkkfrZvdCl3S" src="https://user-images.githubusercontent.com/20363927/229173992-3fe84024-df88-4bb7-bf54-f9f8d91f9191.png">


