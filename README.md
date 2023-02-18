# ActivityPub / Mastodon Ontologies

This ontology is an *unoffical* version of an ActivityPub ontology for experimentation and exploration purposes. It's based on an Activity Streams ontology that was abandoned in favor of JSON-LD in Activity Pub. A separate ontology was created for the Mastodon (toot) extensions.

## Changes to original AS ontology

* Deprecated terms from the original Activity Streams ontology have been removed. 
* Activity Pub extensions have been added to the Activity Streams namespace to be compatible with the Activity Streams JSON-LD context.
* An `Actor` class has been added. Any `Object` with an `inbox` is an `Actor`.
* I've added type-restricted collections (e.g. `OrderedActivityCollection`).
* The OWL range for `as:url` is challenging because the specification defines it as a union of a class (`Object`) and a data type (`xsd::anyURI`). I'm not sure how to model that in OWL or if it's even possible. 

![ontology dendogram](docs/ontology-dendogram.png)

## Disclaimer

I'm not an ontology engineer so I make claims that this is the best way (or even a good one) to represent the ontologies. I'm using this for my own purposes and releasing it in case someone else has a use for it (or wants to collaborate on improving it).





