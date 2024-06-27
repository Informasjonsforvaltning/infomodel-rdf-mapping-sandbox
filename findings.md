# Findings

## RDF Mapping Language (RML)

Virker lovende. Lar en mappe fra heterogene datakilder som XML, CSV og JSON, til RDF.

Virker som mange av elementene i XSD kan uttrykkes av ModellDCAT-AP-NO, men er en del usikkerhet knyttet til dette.

En god del arbeid må legges ned i å skrive RML-definisjonene/mappingene. Kan begynne med å mappe fra XML Schemas. Kan være en utfordring å håndtere gyldige, men vilkårlig utformede XML Schemas på en måte som gir meningsfulle og gyldige RDF-beskrivelser i henhold til ModellDCAT-AP-NO.

### Fordeler

Deklarative definisjoner med RDF Mapping Language, trenger ikke implementere programmer selv for å gjøre mappingen.

Når man først har gjort en mapping er terskelen veldig mye lavere for å lage mappinger som tar andre formater, som JSON/JSON schemas, som input.

### Utfordringer

Noe uvisshet om RML dekker alle behovene, må utforske mulighetene mer.

Er en utfordring å håndtere namespaces i XML og namespaces/QNAMES i RDF. Krever kanskje en viss preprosessering utenfor RML-definisjonene.

## Kilder og verktøy

- [RML: Unofficial draft](https://rml.io/specs/rml/)
- [R2RML: W3C Recommandation](https://www.w3.org/TR/r2rml/)
- [RML mapper Java](https://github.com/RMLio/rmlmapper-java)
- [RML Streamer](https://github.com/RMLio/RMLStreamer)
- [ModellDCAT-AP-NO](https://data.norge.no/specification/modelldcat-ap-no)
