# Java based document search engine using Apache Lucene

Example application which showcases how Apache Lucene can be used in a Java application for indexing and searching documents for keywords.
Apache Tika was used in order to parse the content of multiple file types, including PDF, DOCX etc

## Usage

The app works by using the Lucene Analyzers and Indexer classes. 
Files are parsed using Tika and then indexed. The indexes are stored in a separate folder, then queries are built and then execute.

Lucene uses tranliteration and stemming. 

<img src="https://www.knstek.com/wp-content/uploads/2015/01/lucence-flow-1.png">

## Example usage

Suppose we have multiple documentes containing information about apples. If we index those files and search for "apple", we should receive information about which documents contain information about apples. Stemming means plurals will also be retrieved if we search for the singular and also other words derived from the base word.
Transliteration means that if we search for "mașini", we should also get results containing "masini". Combining the two concepts, we should also get results for "masinile" etc.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[Apache](https://www.apache.org/licenses/LICENSE-2.0)
