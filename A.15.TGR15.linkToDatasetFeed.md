# Download Service feed contains links to dataset feed

**Purpose**: 

Each feed [entry](#entry) in a Download Service Feed shall contain a single [dataset feed link](#datasetfeedlink). This link shall have a "rel" attribute with a value of "alternate" and a "type" attribute with a value "application/atom+xml".

**Test method**

* For each [entry](#entry) in the Download Service Feed, check if exactly one [dataset feed link](#datasetfeedlink) is provided

**Reference(s)**: 

* TG, Req 15

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
entry <a name="entry"></a> | //atom:entry
dataset feed link <a name="datasetfeedlink"></a> | //atom:entry/atom:link[@rel='alternate' and @type='application/atom+xml]/@href