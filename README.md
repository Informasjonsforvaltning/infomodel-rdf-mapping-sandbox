# RDF mapping from XML Schemas to RDF

RML mapping is defined in `./mapping/schema1/schema1-map.ttl`.

Input is the XSD `./mapping/schema1/test.xsd`.

Output is in `./output/schema1/outputtest1.trig`. A prettified format (but without namespaces) in the Turtle file `output/schema1/outputtest1.ttl`.

Requires the a RML Processor, like [rmlmapper-java](https://github.com/RMLio/rmlmapper-java).

To run processor:

```sh
java -cp target/rmlmapper-7.0.0-r373-all.jar be.ugent.rml.cli.Main -m mapping/schema1/schema1-map.ttl -o output/outputtest1.trig -b "http://localhost/"
```
