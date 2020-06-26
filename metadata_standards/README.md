## Metadata Standards and External Resources deployed in the GCIS:
The GCIS conforms with well-established metadata standards and leverages external resources. A list of these is provided below:

## Identifiers:
GCIS makes use of external identifiers such as Digital Object Identifiers ([DOI](https://www.doi.org/)s), [ORCID](https://orcid.org/)s, [ISBN](https://www.isbn.org/about_ISBN_standard)s, [ISSN](http://www.issn.org/)s. ISBN resolution is handled through [WorldCat](https://www.worldcat.org). They may also utilize identifiers created for other aggregator systems, such as [Data.gov](https://www.data.gov/) identifiers. When GCIS must create its own identifier, it may utilize a Universally Unique Identifiers ([UUIDs](https://www.rfc-editor.org/rfc/rfc4122.txt)) when no human-readable identifier is reasonable.

## Provenance:
GCIS utilizes [W3C](https://www.w3.org/Consortium/) provenance to represent some relationships inside the GCIS. In particular, GCIS utilizes [PROV-O](https://www.w3.org/TR/prov-overview/) and [CiTO](http://purl.org/spar/cito) verbs.

## Technology:
GCIS is written in Perl using the Mojolicious web framework, the Rose::DB Database interface, and many other fine modules from the [CPAN](https://www.cpan.org/). It relies on [PostgreSQL](https://www.postgresql.org/about/) for data storage.

Map inserts are supported by [OpenStreetMap](https://www.openstreetmap.org/about) data with [MapBox](https://www.mapbox.com/about/) tiles and implementation through [LeafletJS](https://leafletjs.com/).

## Data Export Formats:
GCIS offers a multitude of human- and machine-readable data export formats, defaulting with the [HTML](https://html.spec.whatwg.org/multipage/) pages. Publication pages can be downloaded as [JSON](https://www.json.org/json-en.html) and [YAML](https://yaml.org/) data, the semantic formats [Turtle](https://www.w3.org/TR/turtle/), [N-Triples](https://www.w3.org/TR/n-triples/), [JSON Triples](https://www.w3.org/wiki/JSON_Triple_Sets), [RDF+XML](https://www.w3.org/TR/rdf-syntax-grammar/), and [RDF+JSON](https://www.w3.org/TR/rdf-json/), and visual representations in [Graphviz](http://graphviz.org/), and [SVG](https://www.w3.org/Graphics/SVG/) of the semantic mapping. Additionally, the data Array(s) behind Table Publications may be downloaded as [CSV](https://tools.ietf.org/html/rfc4180). List pages can be downloaded as JSON, YAML, or CSV formatted data.

## Metadata Quality Characteristics observed in the GCIS:
The Harvard Law School characterizes metadata as “[electronic fingerprints](https://hls.harvard.edu/dept/its/what-is-metadata/)”, that aid the searchability of documents or online resources. Therefore, good metadata records provide users with enough information to understand and (or) locate the object that the record is about.
There is no shortage of qualities that make metadata records “good”. Nevertheless, GCIS metadata records strongly align with the following quality characteristics:

- **Completeness** : Is there enough information to facilitate findability?
- **Conformance**: Do metadata records abide by established standards?
- **Credibility**: Is the metadata based on trustworthy sources?  
- **Readability**: Is the metadata record both machine and human-readable?

The GCIS is designed to aid users in their search for climate science information referenced in USGCRP products. The qualities above reflect this and thus, are central to the GCIS data model. 

