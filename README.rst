MediaWiki Streaming
===================

A set of utilities for stream-processing MediaWiki data.


Usage
-----
    ``mwstream (-h | --help)``
    
    ``mwstream <utility> [-h|--help]``

Data processing utilities
+++++++++++++++++++++++++
    ``diffs2persistence``
        Generates token persistence statistics using revision JSON blobs with
        diff information.
    ``dump2json``
        Converts an XML dump to a stream of revision JSON blobs
    ``json2diffs``
        Computes and adds a "diff" field to a stream of revision JSON blobs
    ``persistence2stats``
        Aggregates a token persistence statistics to revision statistics
    ``wikihadoop2json``
        Converts a Wikihadoop-processed stream of XML pages to JSON blobs

General utilities
+++++++++++++++++
    ``json2tsv``
        Converts a stream of JSON blobs to tab-separated values based a set of
        `fieldnames`.
    ``normalize``
        Normalizes old versions of RevisionDocument json schemas to correspond
        to the most recent schema version.
    ``validate``
        Validates JSON against a provided schema.


Installation
------------

    ``pip install mwstreaming``
