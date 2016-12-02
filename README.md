# KnowledgeFinder

KnowledgeFinder is a open source software to create expert systems, which helps scientists to organize, search and explore their data. Improving their everyday work alone and as a group. 
Documents and their meta data can be automatically crawled, indexed, made searchable and visualized. Interactive and adaptable visualizations allows users to get a quick overview over the stored data and to explore it in depth with just a few clicks.

## Example Use Cases

KnowledgeFinder is a software to create an export system for your needs. Adapt it to your use cases by combining existing features or write your own.

Here is a list of possible use cases which can be adressed by an expert system created based on KnowledgeFinder.

* Get an overview over your data - What data is stored in the expert system? Get a quick overview which data is contained and what it is about by clicking through a graph based representation of your documents based on the provided meta data.
* Learn about a field - Easily get access to all data belonging to specific terms (use full text search and filters). You get a list of the documents including the most important attributes as well as a meta data based visualisation of shared attributes.
* Find out somthing new - Explore the data and look for unexpected or missing connections.
* Search a specific document - The full text search as well as the meta data based filter help you to find the document you search faster.

## Description

The Knowledge Finder allows the classification and indexing of any documents as well as web-based searching for information. Not only full texts are processed but also metadata. These are extracted from the data connections. Possible connections are: SVN, WebDAV, XML, databases, flat files.

So called crawlers are used to extract the metadata from a data source. The crawler uses the interfaces of the corresponding technology of the data source of which the metadata is to be extracted. Has a set of metadata in addition to the metadata attributes a reference to the full text document, the crawler evaluates this reference and importes the related documents. A metadata record is retrieved by the crawler, stored in the Knowledge Finder and prepared for indexing per data entry. The crawling is an offline activity, which is typically ran once a day due to the enormous amount of data in many projects. Then the data can be indexed.

The indexer now processes the metadata and full texts from the respective data sources and writes them into an inverted index. As part of the metadata indexing a metadata model is used. This flexible model represents the structure of the metadata and is used to process the metadata during the indexing and the search process. Each metadata attribute is treated individually in the indexing phase and stored as a separate value in the index. This allows quick filtering of records by metadata attributes. This procedure enables the user interface the display of facets filter based on the metadata attributes. The indexer does its work as well as an offline activity.

After indexing, the search engine can access the index and search the respective databases. For this purpose, this component runs alongside the actual search through the interaction with the user. Here, the processing of the query, the relevance determination, and presentation of results will take place. To perform the search, this component first transformes the information needs of the user in an appropriate form of representation. Subsequently, a search and the subsequent ranking is performed. Recently the search engine presents the result set within the user interface. To generate the facets, the search engine also uses the metadata model.

## Related projects

* [KnowledgeFinder Dataimport](https://github.com/KnowledgeFinder/knowledgefinder-dataimport)
* [KnowledgeFinder Webapp](https://github.com/KnowledgeFinder/knowledgefinder-webapp)

## Set up

The knowledgefinder-core is the basis module of the KnowlegFinder and provides common dependencies for all other submodules. A guide to set up the whole KnowledgeFinder Project including a basic example configuration can be found [here](https://github.com/KnowledgeFinder/knowledgefinder-core/wiki/Quick-Set-up).

## Documentation

The documentation can be found in the [wiki](https://github.com/KnowledgeFinder/knowledgefinder-core/wiki).
