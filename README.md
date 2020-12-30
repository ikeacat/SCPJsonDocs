# SCPJsonDocs
A repository for converted SCP Docs.

## The Breakdown of an article.
Breakdown of a regular article.

### Required (fields that are in every article)
#### title
Title of the article. Ex. Blue Lady Cigarettes

String

#### Item Num
Self explanitory, the item number. Ex. SCP-013

String

#### objClass
The object class.
Ex. Safe

String

#### spcp
Special Containment Procedures

Array of Strings

#### description
Description

Array of Strings

#### lastupdated
The last time the article was updated in the repository

String

#### author
Author of an article (Creater of the page on the wiki). Unknown when it is credited to an IP or The Administrator.

String

### Optional (Fields that are not always present)
#### image
Contains all the images present in an article. See image for the keys that exist and what they do.

Array of Dictionaries

#### addendums
Addendums present in the article. See addendums for the keys that exist and what they do.

## Keys

#### image
url: URL of the image.
caption: The caption under the image.

#### addendums
There will be multiple instances of these dictionaries in the array.

adtitle: Title of the addendum.
paragraphs: Array of strings that make up the addendum.

## Special Files
classLists.json: Contains arrays of links to raw articles that are all of the same object class.
JSONWritingGuide.txt: Useful for when writing a JSON file.
SCPAppConnectionTester.txt: Just to see if downloading from the repo is possible..
byAuthor.json: Dictionary where each key is an array of links to articles that are of the same author. All unknowns are under "Unknown".