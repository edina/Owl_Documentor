#Owl_Documentor

A script to create an HTML page documenting the Ontology.

##Usage

    ./owl_doc my_ontology.rdf > /path/to/web/pages/filename.html

The script parses the rdf document (it currently only understands RDF) specified on the command line and writes to standard out.

##Description


It lists the Classes (and the properties that class accepts), then the Properties (with the Classes the property is a value for)

It also provides a nice relationship map, showing the mapping between Class and Property.

There are three variations on the theme:
* `owl_doc` produces a page with a force-vector diagram for the relationship map (see [example A](examples/ont.html)),
* `owl_doc_chord` produces a page with a chord diagram for the relationship map (see [example B](examples/ont-chord.html)), and
* `owl_doc_bundle` produces a page with a link diagram which highlights the relationship between "has a value" and "is a value of" (see [example C](examples/ont-bundle.html)).


